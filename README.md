# Calculator
This calculator was built to scratch an itch. I wanted a physical RPN calculator similar to the excellent RealCalc. I also wanted an excuse to play around with a pi pico, particuarly their PIO. Finally I wanted a hardware platform to allow me to tinker in firmware and SW as I had ideas and wanted to try something out.

![vanity shot](https://github.com/miket6000/Calculator/assets/7330990/7c552abc-8769-48d4-aa75-e9381a0d92a2)

## Status
### Electrical
The PCB is great all circuits have been tested and I'm not aware of any issues. I'm very impressed with the OLED display (photographing it is hard). 

The pico's lowest standby power is only so-so, I can get down to about 980uA which with the 2500mA battery last around 3 months between charges if you only use standby and not the power switch (and significantly less time if the display is left on).

### Mechanical
The 3d printed enclosure and OLED support are perfectly functional, however I wouldn't mind adding more support in the center of the PCB to help dampen some of the button click noise. 

The front panel is a little iffy. The text is too small to easily read, there's not really enough room to make it larger. I also didn't properly consider the mounting so while I did design it with an assembly method in mind, and it does work, there's room for improvement.

### Software
The software is in a good demonstration state. Standby has been implemented to allow low power measurements. The display drivers and basic screen & keyboard abstraction layers have been created as has the skelaton of the ALU. So today you can use it as a basic pocket calculator. This is only a fraction of what I had planned though. 

I wanted to create a macro system so you could record common equations and adjust the variables you want. There's also a softkey function which so far is barely implemented. One softkey is used to put the calculator into standby, the others need defining and a proper system for assigning actions to the soft keys needs to be built.
