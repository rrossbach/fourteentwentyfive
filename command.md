# Introduction #
[Command](http://code.google.com/p/fourteentwentyfive/source/checkout?repo=command) is the 2012 [BunnyBots](http://www.team1540.org/bunnybots) competition code, built on the FRC CommandBasedRobot template.

This page contains a description of the code foundation, requirements for the code (measurements, patterns framework).

All original information about the [BunnyBots](http://www.team1540.org/bunnybots) (competition, rules, etc. etc.) can be found at the [Team 1540 "Flaming Chickens"](http://www.team1540.org) web site.

# Game Strategy #

The game is divided into two periods, [Autonomous](CommandAutonomous.md) (15 seconds) and [Teleoperated](CommandTeleoperated.md) (the remainder of the round, about 2 1/2 minutes.)

During [Autonomous](CommandAutonomous.md) play, our primary goal is to tip over containers of ping-pong balls placed around the arena and collect as many balls as possible.

During [Teleoperated](CommandTeleoperated.md) play, the drive team will be able to steer the robot to collect additional balls and to deliver the balls to the scoring area.

# Code #

The robot code for this project is available in our 'command' repository.  To build the code, clone the repository to your workspace:
```
git clone https://code.google.com/p/fourteentwentyfive.command command
```
Note that the workspace name is embedded in the Wind River project files, so if your Wind River installation is not in the default location 'C:\WindRiver' or you name the workspace directory anything other than 'command', it won't compile.