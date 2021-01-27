# SerialSensors
A protocol and set of libraries to read sensors via the serial port.  Useful for WebSerial and MCU-MCU comms.

# Goals
AT ATMakers we are consistently finding a need to communicate over basic UART links with no flow control and no significant buffering.  This project is meant to hold solutions to this problem.

# Components
 1. A documented protocol for interfacing with sensors attached to a MCU over a serial link.  Protocol should handle error detection, connection reset, and commands to fetch sensors values, start/stop streaming of values, and start/stop recording of values.
 1. "Host" implementation based on Arduino using TinyUSB when USB Hosting is needed.
 1. "Client" libraries implemented in Arduino, CircuitPython, and Javascript (WebUSB/WebSerial) for pulling data out
