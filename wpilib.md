# Introduction #

Code in this repository is based on the latest 2013 release with modifications for portability to other compilers and other target systems.

# Details #

The bugfixes in this project are essential for proper operation of the 2013 competition project ([holo3](holo3.md)) and the 2013 Bunny Bots project ([bunny](bunny.md)).  Both the bugfixes and portability changes are necessary for the [porting](porting.md) project.

To build, set up the target project and this project in parallel directories (e.g. /c/windriver/workspace/holo3 and /c/windriver/workspace/wpilib).  Import both projects into Workbench using File->Import->Existing Projects Into Workspace.  If all goes well, this wpilib project will be set up as a dependency of the target project.  Running Project->Build on the target project should build wpilib and then the target project and finally link them into a ".out" file.