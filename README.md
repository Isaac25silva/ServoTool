[![Build Status](https://travis-ci.org/Isaac25silva/ServoTool.svg?branch=master)](https://travis-ci.org/Isaac25silva/ServoTool)

ServoTool
=========

Code released by Team Darmstadt Dribblers in the RoboCup humanoid league website: https://www.robocuphumanoid.org/materials/open-source/


This code is in the repository on github: https://github.com/DorianScholz/ServoTool


A GUI tool written in Python and Qt to configure and analyze different servo motors (mainly the ones made by Robotis, INC).
It's primary aim was to provide a cross platform tool running on Linux, OSX and Windows.
Besides offering an overview of the connected servo motors and their current configuration in a table view it provides a 2D plot to visualize motor data.

Dependencies
============
```
sudo apt-get install python-serial python-qwt5-qt4
```

Usage
=====
* run 'python src/ServoTool.py'
* select the correct protocol, port and baudrate
  * usually 'RobotisServo', '/dev/ttyUSB0' and '57600'
* click the 'Read All' button which will connect to serial, scan for servos and read all data from them
  * you should see all connected servos in the table view and can edit their data
* if it does not work check the log view on the bottom for errors
