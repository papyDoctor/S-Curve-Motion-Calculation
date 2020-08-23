# S-Curve-Motion-Calculation
Can be tested here https://mybinder.org/v2/gh/papyDoctor/S-Curve-Motion-Calculation/master

(ALWAYS begin execution from the FIRST cell. Do twice the entire sheet to have graphics in good format)

Discussions about this calculation on https://groups.google.com/g/openpnp/c/YBS0a3vZEAw

*UPDATE:* Special thanks to _Mark from OpenPnP group for having tested the first version of this calculation and shown that it was not optimal.

This jupyter notebook shows a way to calculate the complete S-Curve motion without any iteration.

**Given maximum jerk-acceleration-speed, given xStart and xEnd, the algorithm calculates the travel that uses the minimum time**

S-Curve motion means that, given the speed, acceleration and hyper-acceleration (called jerk), given a starting and a ending point, the calculation results give a smooth motion: at any time the jerk is maintained under a given maximum.

During the travel, a S-Curve motion can take up to 7 phases. Depending of the parameters, the phases may be lowered until 4.
