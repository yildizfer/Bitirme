Project: Bitirme

This project contains a quaternion-based state estimator designed by ouafi98, parametrized hyperbolic tangent based generalized angular velocity reference signal, fuzzy PD controllers to track this reference and cascaded PID controllers to correct any remaining attitude errors alongside with default position controllers.

The minidrone can perform up to two consecutive flips around the roll axis and one around the pitch axis with the given controller parameters.
The gain vector can be modified to change flipping axis.
The number of flips n is specified inside the reference generation function block.
For n>1 the altitude reference should also be set accordingly due to the physical limitations of the system.
The time when the attitude controllers are disabled and the default position controllers are enabled is specified as tdisable. This parameter can be subjected to further optimization.