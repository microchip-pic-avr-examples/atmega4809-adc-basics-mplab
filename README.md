<a href="https://www.microchip.com" rel="nofollow"><img src="images/microchip.png" alt="MCHP" width="300"/></a>

# ATmega4809 Xplained Pro ADC basics

MegaAVR® 0-series devices feature a 10-bit successive approximation register (SAR) Analog-to-Digital Converter (ADC) and is capable of conversion rates up to 115 ksps. It features a flexible multiplexer, which allows the ADC to measure the voltage at multiplesingle-ended input pins.

There are four modes we will explore in this example:
*  ADC Free-Running mode
*  ADC Single Conversion mode
*  ADC Window Comparator mode
*  ADC Sample Accumulator mode

This is an example of how to get started with the ADC on the ATmega4809. This is based on the application note [AN2573](https://www.microchip.com/wwwAppNotes/AppNotes.aspx?appnote=en601379).

## Related Documentation

- [AN2573 - ADC Basics with tinyAVR 0- and 1-series, and megaAVR 0-series](https://www.microchip.com/wwwAppNotes/AppNotes.aspx?appnote=en601379)
- [ATmega4809 Device Page](https://www.microchip.com/wwwproducts/en/ATMEGA4809)

## Software Used

- [MPLAB X IDE v5.40 or later](https://www.microchip.com/mplab/mplab-x-ide)
- Data Visualizer
    - [MPLAB Data Visualizer](https://gallery.microchip.com/packages/MPLAB-Data-Visualizer-Standalone(Windows)/)
    - [Studio Data visualizer](https://www.microchip.com/mplab/avr-support/data-visualizer)
- [XC8 (v2.20)](https://www.microchip.com/mplab/compilers) alternatively [AVR/GNU C Compiler 5.4.0](https://www.microchip.com/mplab/avr-support/avr-and-arm-toolchains-c-compilers) can be used
- ATmega_DFP 2.2.108 or later

## Hardware Used

- [ATmega4809 Xplained Pro](https://www.microchip.com/developmenttools/ProductDetails/ATMEGA4809-XPRO)

## Setup

* Port `PD6` is the ADC channel input, connect a cable here to interract with the ADC

## Operation

1. Download the zip file or clone the example to get the source code.
2. Open `atmega4809-adc-basics-mplab.X` in MPLAB.
3. Connect the ATmega4809 Xplained Pro to your computer with a micro usb cable.
4. Make sure the kit is selected as the tool to be programmed under project settings.
5. Press the make and program button to program the device.
6. Open your favorite terminal application or Data visualizer and open the serial port associated with the Xplained Pro.

As mentioned in the appnote [AN2573](https://www.microchip.com/wwwAppNotes/AppNotes.aspx?appnote=en601379) you can change the voltage level of the adc input port and the approximated value will be shown over UART through data visualizer.

## Conclusion

We have here shown how to setup and get started with the ADC basics project. For more details about this example and how the ADC works please see the [AN2573](https://www.microchip.com/wwwAppNotes/AppNotes.aspx?appnote=en601379) Application Note.