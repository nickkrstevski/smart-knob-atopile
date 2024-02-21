# smart-knob
Shoutout to Scott Bezek for creating this awesome open source haptic feedback wheel!
https://github.com/scottbez1/smartknob.git

# atopile
>ato install smartknob

This package contains adaptations of the smart knob designs captured in atopile code. atopile will help with jellybean component selection, board layout, versioning, collaboration..

Upon importing the smart knob package into your atopile project, you will find a complete netlist and accompanying layout that can be merged or connected into a larger design. atopile's component selection integrates directly wih the JLC component supplier, generating build outputs that can be directly sent to JLC and show up at your door assembled.

For example, I am creating a chess clock that uses the smart knob as a dial, and adds some leds/capacitive touch sensors to build upon the original design/layout.
https://github.com/nickkrstevski/chess-clock

# Structure
The Smart Knob design consists of 2 PCBAs, a BLDC motor, an LCD, and plenty of mechanical bits holding everything together. This project will contain a Smart Knob module that has 2 build target modules, "SmartKnobBase", and "SmartKnobScreen"

## SmartKnobBase
- ESP32-S3
- USB-C
- BLDC Driver
- Strain Sensor
- Ambient Light Sensor
- Magnetic Quadrature Encoder

## SmartKnobScreen
- Backlight FET/ballast resistor
- LCD Connections