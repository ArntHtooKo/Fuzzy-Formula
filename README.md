The inverted pendulum is a classic control problem: a pole attached to a moving cart must be held upright using only horizontal force. Without control, it falls immediately due to gravity.

This project designs a fuzzy logic controller that stabilizes the pole for small to moderate disturbances.


Objectives
Implement a dynamic simulation of an inverted pendulum

Design and apply a fuzzy logic controller

Demonstrate stabilization for small to moderate disturbances

Generate and analyze a fuzzy control surface

Discuss system limitations




System Model
State variables:

Cart position

Cart velocity

Pole angle

Pole angular velocity

Control input: Horizontal force applied to the cart

The dynamics are based on Newtonian mechanics, with coupled nonlinear equations for horizontal and angular acceleration. A fixed timestep integrates the equations numerically.





Fuzzy Logic Controller
Component	Details
Inputs	Pole angle, angular velocity
Output	Horizontal force on cart
Linguistic terms	Negative Large, Negative Small, Zero, Positive Small, Positive Large
Rule base	25 rules (5×5)
Core principle: Move the cart in the same direction as the falling pole to reposition under the center of mass.

Arnt Htoo Ko
Bachelor of Information Science — Double Major in IT & Computer Science
