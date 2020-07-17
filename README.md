Cmod A7-35T GPIO Demo
==============

Description
--------------
This project is a Vivado demo using the Cmod A7's LEDs, RGB LED's, pushbuttons, and USB UART bridge, written in VHDL. When programmed onto the board, the pushbuttons are tied to the LEDs. Every time a button is pressed, the corresponding LED will light up. The RGB LED smoothly transitions between colors.

To use the USB-UART bridge feature of this demo, the Cmod A7-35T must be connected to a serial terminal on the computer it is connected to over the MicroUSB cable. For more information on how to set up and use a serial terminal, such as Tera Term or PuTTY, refer to [this tutorial](https://reference.digilentinc.com/learn/programmable-logic/tutorials/tera-term). On reset, the Cmod A7-35T sends the line “CMOD A7 GPIO/UART DEMO!” to the serial terminal. Whenever one of the buttons is pressed, the line “Button press detected!” is sent.

Requirements
--------------
* **Cmod A7-35T**:To purchase a Cmod A7-35T, see the [Digilent Store](https://store.digilentinc.com/cmod-a7-breadboardable-artix-7-fpga-module/)
* **Vivado 2020.1 Installation**:To set up Vivado, see the [Installing Vivado and Digilent Board Files Tutorial](https://reference.digilentinc.com/vivado/installing-vivado/start).
* **Serial Terminal Emulator Application**: For more information see the [Installing and Using a Terminal Emulator Tutorial](https://reference.digilentinc.com/learn/programmable-logic/tutorials/tera-term).
* **MicroUSB Cable**
 
Demo Setup
--------------
1. Download and extract the most recent release ZIP archive from this repository's [Releases Page](https://github.com/Digilent/Cmod-A7-35T-GPIO/releases).
2. Open the project in Vivado 2020.1 by double clicking on the included XPR file found at "\<archive extracted location\>/vivado_proj/Cmod-A7-35T-GPIO.xpr".
3. In the Flow Navigator panel on the left side of the Vivado window, click **Open Hardware Manager**.
4. Plug the Cmod A7-35T into the computer using a MicroUSB cable.
5. Open a serial terminal emulator (such as TeraTerm) and connect it to the Cmod A7-35T's serial port, using a baud rate of 9600.
6. In the green bar at the top of the Vivado window, click **Open target**. Select **Auto connect** from the drop down menu.
7. In the green bar at the top of the Vivado window, click **Program device**.
8. In the Program Device Wizard, enter "\<archive extracted location\>vivado_proj/Cmod-A7-35T-GPIO.runs/impl_1/GPIO.bit" into the "Bitstream file" field. Then click **Program**.
9. The demo will now be programmed onto the Cmod A7-35T. See the Description section of this README to learn how to interact with this demo.

Next Steps
--------------
This demo can be used as a basis for other projects, either by adding sources included in the demo's release to those projects, or by modifying the sources in the release project.

Check out the Cmod A7-35T's [Resource Center](https://reference.digilentinc.com/reference/programmable-logic/cmod-a7/start) to find more documentation, demos, and tutorials.

For technical support or questions, please post on the [Digilent Forum](https://forum.digilentinc.com).

Additional Notes
--------------
For more information on how this project is version controlled, refer to the [Digilent Vivado Scripts Repository](https://github.com/digilent/digilent-vivado-scripts)

