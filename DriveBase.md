# Introduction #

The DriveBase Subsystem represents the basic moving platform of the robot.

# Details #

DriveBase contains three PWM motor controllers [e.g. Jaguar] and a turn-rate gyro connected to an AnalogChannel.  Each of these components must be instantiated by the main Robot (or RobotMap) instance, then provided to the DriveBase constructor.  Robot (RobotMap) class need only create the singleton instances of each motor and the analog channel and connect them to the LiveWindow.  DriveBase then handles any specialized initialization for its components.  For example, it configures the AnalogChannel as needed for input from the MEMS gyroscope.

DriveBase wraps the three motor controllers in an instance of RobotDrive3 which handles the calculations to convert Cartesian drive coordinates to the necessary motor speeds.  DriveBase adds a twist correction from the gyroscope to keep the platform driving straight despite mechanical imbalances and wheel slippage.


# To Be Done #

The current implementation is suitable for a demonstration, but we need to adjust the scaling of the "twist" input from the joystick and the negative feedback from the gyro for a better drive feel.

The gyro channel initialization and the zero-offset calibration value should be encapsulated in their own RateGyro class.


[<<top](Holo3.md)