# ESP-P113
 Compact version of ESP's Project 113 Amplifier done with SMT resistors and ceramic caps. PSU idea taken from https://theslowdiyer.wordpress.com/2019/09/10/project-files-filtered-irm-power-supplies-part-1/. Designed to go in sideways in this case (https://item.taobao.com/item.htm?id=54329725614). 

 ## Changelog
* 25/05/2021: Initial commit.
* 26/05/2021: Updated to V1.1. Added primary-side fuse, changed inductor to cheaper variant and rearranged components to make board even more compact. Updated BOM to match. Added extra M3 hole in middle of PCB and changed that hole to be the case grounding point instead.
* 27/05/2021: Updated to V1.2. Slightly changed position of transistors to allow for them to be mounted to an aluminium L-bracket and then to the case. 3mm power LEDs added. Changed output resistors to THT 0.5W versions. Added disclaimer on board. Moved position of components in CLC filter for more optimal routing.
* 29/05/2021: Updated to V2.0. Added zobel network on outputs, cap between input and outputs of opamp, and rc network on opamp inputs to improve amp stability. Fixed major error with transistors (used wrong symbols/wrong way round, oops!). Added varistor between each power supply input and 3R resistor in series into live input, changed capacitor layout in output and added TVS diode to protect electronics in case converter fails as per CUI PSK-20D datasheet. 3.15A fuses into each live input will also be added off-board in the final design. Added gain switchs to toggle gain resistance between 3k3 and 9k1 by switching 5k1 resistor in and out of parallel (actual resistance with both resistors in parallel is around 3k27, close enough), with option to choose between on-board DIP switches and off-board headers to use another switch. Added Y2 cap between PE and ground to suppress ground loop noise. Completely new layout, slightly larger but should still fit in planned case. Many thanks to user AnalogSteph on ASR for the help on the majority of the changes.

 ## Photos
![Schematic](Amp_PSU/Images/Schem.png)
![PCB Traces](Amp_PSU/Images/PCB_Traces.png)
![Top PCB](Amp_PSU/Images/PCB_Top.png)
![Bottom PCB](Amp_PSU/Images/PCB_Bottom.png)
![Top Render](Amp_PSU/Images/Render_Top.png)
![Bottom Render](Amp_PSU/Images/Render_Bottom.png)