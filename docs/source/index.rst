=========================
Accelerometer Test Module
=========================
QK-05-034
                               
.. figure:: images/kberry-front-photo.png
    :width: 400
    :align: center

    Kooka Accelerator Module



Description
-----------
The Accelerometer Test Module is designed to measure acceleration in three dimensions.  
It contains a Raspberry P1 microprocessor RP2040 coupled to an accelerometer LSM303C.  
The module contains an 80 mAH battery, USB-C connectivity to a PC plus a push button and LEDs connected to the RP2040

Specification
-------------

A Table to be inserted

The *Table* goes **here**.



Application
-----------

The module can be used to measure acceleration in three dimensions



Module Description
------------------

The module has been designed as a subset of the Kookaberry and as such can run the Kookaberry firmware and make use of the IDE features in the KookaSuite -  
being the KookaIDE, KookaBlockly and the KookaTW.  The latest version of KookaSuite can be downloaded from Github at 
https://github.com/kookaberry/kooka-releases/tree/master/KookaSuite


The RP2040 microcontroller is connected to the USB-C and is supported by 3MB of memory and a 12MHz crystal. It operates at 3.2 volts

The on board LIR2032 3.6 volt Li-Ion battery is charged via  Vbus (5 volts) from the USB-C connector and the Power Management circuit which also regulates the module voltage VCC to 3.2 volts

Two jumpers (JP2 and JP3) allow the battery to be connected to the module.  With the jumper in the J2 position the battery is not connected to the module.  With the jumper in the J3 position the battery is connected, it can be charged via the USB-C and it can also supply power to the board if the USB-C is not connected.


A green LED shows when power is connected to the board.  When the board is connected via the USB-C connector to a PC and the battery is connected via jumper J3 the

•	green LED will show power
•	the Power Management blue LED will show charging of the battery and
•	the orange LED will show when the battery is charged


The LSM303 is an accelerometer / Magnetometer integrated circuit.  It is connected to the RP2040 via an I2C bus and provides magnetic and acceleration readings in three dimensions

The Soft Reset button is a feature of the Kookaberry firmware and when pushed provides a software reset to the Kookaberry firmware./ applications

There are two user accessible LEDs (Red and Orange) plus a push button




Mapping
-------




Sample Code - Using KookaBlockly and KookaIDE

KookaBlockly Script to Flash the Red and Orange LEDs


KookaIDE - MicroPython Script to Flash Red and Orange LEDs











KookaBlockly Script to test Push Button




KookaIDE - MicroPython Script to test Push Button


KookaBlockly Script to test LSM303 Acceleration
















KookaIDE - MicroPython Script to test LSM303 Acceleration


Typical Display



