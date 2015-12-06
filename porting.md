# Introduction #

Port robot code and WPILib to other hardware and operating systems so that we can develop and debug code in a friendlier and less expensive environment.

# Details #

There are several parts to the code here:
  * WPILib, modified only where absolutely necessary to allow compilation under gcc4, operation under Linux or Linux-like operating systems (cygwin) and little-endian (e.g. x86) targets
  * replacements or stubs for FRCNetworkCommunications and other robot components that aren't distributed in source form
  * runtime start-up (main)
  * sample robot code, in this case based on our 'holo3' project
  * a WireShark extension to decode packets between the driver station and robot

# Status #

The code compiles and runs under cygwin, x86 Linux and on Raspberry Pi.  The replacement FRCNetworkCommunication module will connect to and exchange control/status information with a driver station, although there seem to be some problems with e.g. the driver station LCD extensions.  The classes that normally talk to the NI FPGA and modules are stubs.  They could be exended to talk to real hardware on e.g. a Raspberry Pi's GPIO pins.