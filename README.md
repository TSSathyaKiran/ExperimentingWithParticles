# Particles with js

## 1:

(initial trial with only 4 particles and fixed positions, have to fix velocity)
![Screenshot 2025-04-27 144737](https://github.com/user-attachments/assets/c255d973-f565-4254-91fe-7cd796a74b21)
![Screenshot 2025-04-27 144751](https://github.com/user-attachments/assets/5aa901d9-2c3d-47ea-ab31-370157bdc7df)


## 2:

(fixed velocity and added buttons on the side to run, stop and reset)
![Screenshot 2025-04-28 224356](https://github.com/user-attachments/assets/85b6bf89-0721-4ff9-b0aa-8b5d12bbfae3)
![Screenshot 2025-04-28 224438](https://github.com/user-attachments/assets/a252547c-988a-413d-89de-3e6dbfa29fde)


## 3:

(added random spawns for different colours, js cant handle too many sadge)
![Screenshot 2025-05-01 122741](https://github.com/user-attachments/assets/763bf26b-5535-4d69-8aa2-6ac13a234905)
![Screenshot 2025-05-01 122751](https://github.com/user-attachments/assets/6a008dd7-7d41-46c6-856a-1a2633cdeddc)

(have to add buttons and sliders to adjust values of each particle on the page directly)

---

-- you can change each set of particle in the code

``` javascript

        // color = Random_Particles(number, color-name)

        yellow = Random_Particles(300, "yellow")
        blue = Random_Particles(150, "blue")
        red = Random_Particles(270, "red")
        green = Random_Particles(180, "green")

```

-- you can change how each particle interacts with each other as well

``` javascript

            // force(Particle1, Particle2, Force-Multiplier, Radius, Velocity-Multiplier)
            // Force-Multiplier: negtive for attraction and positive for repulsion
            // Radius: how far each particle checks 
            // Velocity-Multiplier: multiplier for velocity of particle1 w.r.t particle2

            force(red, red, -0.174, 80, 0.5)
            force(blue, red, -0.098, 100, .6)
            force(red, green, -0.1, 78, 1.7)
            force(green, yellow, -0.111, 120, .5)
            force(blue, yellow, 0.1, 70, 1.5)
            force(red, blue, 0.0923, 112, 1)
            force(yellow, red, -0.0789, 100, .6)
            force(green, green, 0.132, 85, .71)
            force(yellow, blue, 0.1, 78, .6)

```