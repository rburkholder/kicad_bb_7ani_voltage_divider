# BeagleBone Black/Green Cape for Voltage Divider based Analog Input for 7 channels.

* Current version supports thermister and LDR (light dependent resister)
* The book "Exploring BeagleBone®: Tools and Techniques for Building with Embedded Linux®, Second Edition" by Derek Molloy is the source of inspiration
* Relevant Pages include:
  * page 178 - 181 Operational Amplifiers - voltage source, voltage follower, buffer
  * page 248 - 249 Interface Ports
  * page 280 - 282 Analog Inputs, how to read
  * page 282 - 284 unbuffered light meter voltage divider
  * page 420 - 426 buffering analog input
  * page 427 - 431 voltage division & scaling with op-amp included


In effect:
* the two op-amp MCP6002 provides a buffered 1.8V rail-to-rail output for use by the voltage dividers
* the eight op-amp MCP6004 provides a rail-to-rail voltage follower to provide high input impedance for the voltage divider, and low output impedance to the BB analog input pins

Results, as of 2025/12/26 - not etched yet:
* ![Schematic](pictures/Screenshot_20251226_213154.png)
* ![Printed Circuit Board](pictures/Screenshot_20251226_213255.png)

