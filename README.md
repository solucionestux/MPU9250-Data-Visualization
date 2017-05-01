# MPU9250-Data-Visualization
A useful tool to visualize at real time data of the MPU9250 sent through a COM port

The MPU-9250 is a sensor from Invensense Inc that combine in one package both accelerometer, gyroscope and magnetometer. It embeds also a thermometer and other useful things. [The datasheet can be found here.](https://store.invensense.com/ProductDetail/MPU-9250-InvenSense-Inc/487537/pid=1135)

Repository Contents
-------------------

* **/Libraries** &mdash; An Arduino library (from sparkfun)
* **/acq_mpu9250** &mdash; The Arduino code to send data to a COM port
* **mpuScrollingPlot.py**; A Python script for "scrolling plotting"
* **mpuPlotSavedData.py**; to visualize saved data

Required Python Package
-----------------------

- import serial
- import time
- import numpy as np
- from matplotlib import pyplot as plt
- import pyqtgraph as pg
- from pyqtgraph.Qt import QtCore, QtGui
- import os
- import pyqtgraph.console
- import PyQt5

Sending data to a COM port
--------------------------

I use an Arduino board. Here is how I do it

![wiring] (https://github.com/Sanahm/MPU9250-Data-Visualization/wiring.png)

Results
-------

![Data's visualization interface] (https://github.com/Sanahm/MPU9250-Data-Visualization/visu.png)

The script mpuPlotSavedData.py allows you to plot the saved data using matplotlib

![Visualize saved's data] (https://github.com/Sanahm/MPU9250-Data-Visualization/plotSaved.png)
