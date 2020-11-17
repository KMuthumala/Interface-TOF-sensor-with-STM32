

# VL53L0X library for STM32 MCUs
This is a edited version of the arduino library provided by . 
The original Arduino library can be found at here.[VL53L0X time-of-flight distance sensor Arduino library](https://github.com/pololu/vl53l0x-arduino)
## Supported platforms

This is compatible with Atollic Studio IDE and Eclipse based other platforms.
## Getting started

### Hardware

A [VL53L0X carrier](https://www.pololu.com/product/2490) can be purchased from Pololu's website.  Before continuing, careful reading of the [product page](https://www.pololu.com/product/2490) as well as the VL53L0X datasheet is recommended.


#### Connection

(including Arduino Uno, Leonardo, Mega; Pololu A-Star 32U4)

    STM32   VL53L0X board
    -------   -------------
     3.3/5V - VIN
        GND - GND
        SDA - SDA
        SCL - SCL

## ST's VL53L0X API and this library

Most of the functionality of this library is based on the [VL53L0X API](http://www.st.com/content/st_com/en/products/embedded-software/proximity-sensors-software/stsw-img005.html) provided by ST (STSW-IMG005), and some of the explanatory comments in the code are quoted or paraphrased from the API source code, API user manual (UM2039), and the VL53L0X datasheet. For more explanation about the library code and how it was derived from the API, see the comments in VL53L0X.cpp.

This library is intended to provide a quicker and easier way to get started using the VL53L0X with an STM32-compatible controller, in contrast to customizing and compiling ST's API for the STM32. The library has a more streamlined interface, as well as smaller storage and memory footprints. However, it does not implement some of the more advanced functionality available in the API (for example, calibrating the sensor to work well under a cover glass), and it has less robust error checking. For advanced applications, especially when storage and memory are less of an issue, consider using the VL53L0X API directly.

## Library reference

References can be found at the original Arduino library. [here](https://github.com/pololu/vl53l0x-arduino)






