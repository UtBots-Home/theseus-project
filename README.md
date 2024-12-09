# THESEUS: Build, adapt, and evolve with an open-source manipulator

Built for modularity and scalability, the Theseus arm is in its first phase of field testing.
Our main objectives are constructing a manipulator that can deliver decent accuracy for simple household tasks, that can be built on a budget, yet can still lift a relatively high payload when compared to its peers in the @home category of CBR.

![Screenshot from 2024-12-09 10-43-31](https://github.com/user-attachments/assets/fd263ef9-30d8-498e-b453-c7a902157ff5)

## Making it move: selection of motors and actuator design

To get reliably strong and fast motors without breaking the bank, 8318 type outrunner brushless motors, commonly used in medium to large drones, were chosen for the main actuators. Also for budget reasons some other motors were mixed in. Namely a 30 KV standard hoverboard motor and a few MG 995r servos for other joints. Save for bthe servos, all other motors were coupled to a custom-made 25:1 cycloidal gearbox, via a 2:1 belt and pulley system. Raising the total torque of the motors by a factor of 50. The cycloidal reducers are currently printed in standard ABS plastic due to its ease of post-processing, and, while keeping the cost down, causes the actuators to fail at the axis part before reaching maximum force output. However this isn't a concern seen as the effective output is already significantly higher than required for the tasks.

The gearboxes were designed for ease of printing in 7 parts (plus 5 non-printed ball bearings and a few screws). The cad models can be found at the ./models folder and while relatively simple, it can be a hassle to get the tolerances right on different printers. We found the device works best when the cycloidal discs sit snugly within the shell, easily spinning as the axle is turned, but tight enouh not to fall off with a couple shakes. The actuators require a few non-prtinted parts which are relatively cheap and easy to find:

- 4 M4 screws and matching nuts to clamp it all together
- 2 12 x 18 x 4 bearings for the eccentric axle
- 2 8 x 22 x 8 bearings to keep the axle straight
- 1 25 x 37 x8 bearing for the output shaft

at time of purchase, these parts amounted to less than 50 BRL. Which, for our non-brazilian friends is just under than 60 CNY, and well under 10 USD
