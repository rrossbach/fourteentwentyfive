# Introduction #

'Holo3' started as a demonstration project for a 3-wheeled holonomic drive platform and grew to become the 2013 competition robot.

# Details #

Most of this code is just a CommandBasedRobot wrapper around the DriveBase, Shooter and Climber subsystems.  There's also a BlinkyLight that can be used to demonstrate simple state machine development.

The DriveBase subsystem is built around the [RobotDrive3](RobotDrive3.md) class, derived from the WPILib RobotDrive class.  RobotDrive supports both 2-wheel and 4-wheel platforms; [RobotDrive3](RobotDrive3.md) adds a constructor for 3-wheel platforms and a new drive method that handles the conversion from Cartesian coordinates to 120-degree drive.

# Post-Season Update #

The "master" branch is the code we used in competition.  The "stevet" branch contains post-season bugfixes to the Autonomous-mode code.  It must be built with along with our modified [wpilib](wpilib.md) project; see that project's Wiki page for instructions.