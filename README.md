# Storm Alert

A mobile barometer designed for notification of rapidly approaching storms in the mountains.
Uses GPS to obtain elevation data to compensate for dropping pressure during altitude gain. Stores two sets of pressure data and looks for a rapid drop in pressure.

NOTE: There is a threshold set for the pressure drop to determine when to alert for a potential storm. This threshold value is experimental and might not be correct. The mountains are a dangerous place and one should not rely on this device to keep them from harm.

## Hardware:
 * Arduino Nano (or compatible micro-controller)
 * NEO-6M compatible gps sensor. Tx to pin 8, Rx to pin 9
 * BMP180 barometer/thermometer. SCL to pin A5. SDA to pin A4;
 * SSD1306 128X64 compatible SPI OLED screen. Clock/D0 to pin D3, Data/D1 to pin D2, CS to pin D5, DC to pin D4, Reset to pin D13);
 * Active buzzer with PN2222 transistor connected to pin D6. PN2222 connections: Emitter to +5V, Base to Arduino D6, Collector to to active buzzer

For more info on the hardware connections, checkout the Fritzing wiring diagram.

## Software:
  * Developed in the Arduino variant of C/C++
  * Uses the following libraries (make sure you have them installed)
   * Wire
   * SFE BMP180
   * AltSoftSerial
   * TinyGPSPlus
   * SPI
   * U8g2


Released under the MIT license. Have fun!

V1.0 Halcy Webster - 16DEC2017
