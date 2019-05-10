# robotc-elevator
Code for an elevator I made using VEX and ROBOTC

This code was written for the VEX ROBOTC platform. Unless you either modify the code, it probably won't work on anything that isn't the specific elevator it was designed for.

## How it works
The elevator itself is powered by a single motor on a chain. The chain both pulls the car both up and down, since gravity isn't strong enough to prevent the car from wobbling around and getting jammed. A single optical shaft encoder determines the position of the car by measuring the rotation of the motor axle.

The code works by running an infinite loop indefinetly. There are two if-else blocks within the while loop. The first one monitors the elevator buttons and sets a variable to the target value if a button is pressed. The second sets the motor either in either forward, reverse, or stop depending on the encoder's value relative to the target. The second one also slows down the motor once the car is close to the target.

---

Credit to @ChuckCleason for leading the mechanical design.
