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

