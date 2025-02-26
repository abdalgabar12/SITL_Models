These models are quad X-frame copter tailsitters contributed by Otto Kueng and based on the actual flying model by Pierre Losa:

![BiWing image](https://github.com/ArduPilot/SITL_Models/blob/master/RealFlight/WIP/markw/Tailsitters/CopterTailsitters/BiWing/BiWing_JWL065.jpg)

[BiWing Tailsitter video](https://youtu.be/3nS2AodrGPQ)

The copter tailsitter quad-X frame class and type are specified by:<br />
Q_FRAME_CLASS = 1<br />
Q_FRAME_TYPE = 1<br />
and<br />
Q_TAILSIT_MOTMX = 15 = 0b1111 to enable all 4 motors in FW modes<br />
or<br />
Q_TAILSIT_MOTMX =  5 = 0b0101 to enable only the bottom wing motors<br />
or<br />
Q_TAILSIT_MOTMX = 10 = 0b1010 to enable only the top wing motors


PR https://github.com/ArduPilot/ardupilot/pull/12869 is required for multicopter frame yaw control (body-frame roll) to work correctly when hovering.

Model BiWing_JWL065_EA.RFX has airfoil and CG similar to the actual flying model by Pierre Losa.

Model BiWing_MH106_EA.RFX has a symmetrical airfoil with CG moved further back for comparison of aerodynamic characteristics. 

These models have been tested in RealFlight8 with the parameters in file: BiWing.parm
