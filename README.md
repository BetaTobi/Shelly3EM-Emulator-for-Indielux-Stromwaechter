# Shelly3EM-Emulator-for-indielux-Stromwaechter

The "Shelly3M Emulator for indielux Stromwächter" offers the possibility to install and use the "Stromwächter" from the company indielux GmbH without having the “real” (physical) Shelly3EM device available.

Today (summer of 2024), it is mandatory to have a Shelly3EM device installed in your in-house fuse-box, to be able to fully use all features of the Stromwächter.
Nevertheless, it is possible to emulate the Shelly3EM device and to distribute the necessary data (values of current, voltage, power…) via other hardware and/or software sources.

Currently, the Shelly3EM emulator is available for
+ Node-RED
+ Arduino IDE



## What you need…

### In any case:
+ Data of your fuse-box for all three phases (L1, L2, L3)
  + Current (in A)
  + Voltage (in V)
  + Power (in W)
  + Powerfactor (dimensionless)
+ All data available as MQTT topics (independent on their origin)

### For the Node-RED solution:
+ Some hardware, where Node-RED can be installed (Raspberry Pi, Notebook…)
+ Node-RED software (https://nodered.org/ )

### For the Arduino IDE solution
+ Any ESP32 microcontroller (e.g. https://www.az-delivery.de/products/esp-32-dev-kit-c-v4 )
+ Arduino Ide software (https://www.arduino.cc/en/software )



## How to…

The installation guides for the different options can be found in the related Wiki articles.

https://github.com/BetaTobi/Shelly3EM-Emulator-for-indielux-Stromwaechter/wiki

The installation guide for the Stromwächter can be found here:

https://www.indielux.com/support/anleitungen/indielux-ready2plugin-stromwaechter-anleitung/#stromwaechter-bedienung


## Note:

The Stromwächter uses the MQTT-values (or more correct, the values coming from the Shelly3EM) for health monitoring of the whole system and is able to cut-off the electrical system, if it detects an issue (e.g. no more updated values of power, current, voltage… available). 

Do not manipulate the values in such a way, that they are not reflecting the current status of your “real” system. Otherwise, it might be possible, that the safety system of the Stromwächter can be undermined.
