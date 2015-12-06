# Introduction #

After the first 15 seconds of the competition round, the drive team can use the joystick and switches on the operator interface (aka DriveStation) to control the robot.

# Functions #

The robot will have a ball collector with an opening along one of the longer edges of the drive base.  Forward motion of the operator's joystick should move the robot toward this edge so that it can pick up balls.

The ball collector will have a roller which helps it pick up or release balls.  The driver must be able to turn the roller motor on and off and change its direction.

The ball collection tray will be raised and lowered by a double-acting air cylinder controlled by two outputs from the pneumatics module.  The tray must be lowered to collect or discharge balls.  It may be raised to hold balls already collected or to help clear obstacles on the floor (such as the scoring areas).

# Operator Controls #

## Drive Base ##

Normal motion of the robot will be controlled by the joystick X/Y/Twist axes with the maximum speed in each direction set by the joystick throttle control.

The robot may be locked into motion along any one of the four primary directions by pushing the joystick in that direction, then pulling the joystick trigger.  _Hint: Set the throttle to minimum before doing this._  The robot will move only in that direction with speed controlled by the throttle control until the direction is changed by moving the joystick and pulling the trigger again.  Pulling the trigger while the joystick is at (or near) the center position will return the robot to normal joystick control.

The first line of the driver station display will display the current operation mode: "joystick", "forward", "reverse", "right" or "left".

## Ball Collector ##

The ball collector and tray will be controlled by three buttons on the driver joystick:

Button 3 (top left) lowers the tray and starts the collector motor running "forward" (collecting balls.)

Button 4 (top right) lowers the tray and starts the collector motor running "backward" (dumping balls.)

Button 2 (bottom center) stops the collector motor and raises the tray.


