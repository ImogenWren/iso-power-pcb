# ISOpowerProject
 Remote power control board for ISO experiment containers, used for remote labs projects
![ISOpower](https://user-images.githubusercontent.com/97303986/158610534-c0feec4a-f649-47c7-bc71-ae8b51f817a3.png)
![ISOpowerPCBdesign](https://user-images.githubusercontent.com/97303986/158610818-84cbbe2c-e711-4a15-b655-8e105aa62b4e.png)

## Use

### Programming [See Issues]
 To Program AtMega328pb use the following settings:
 ![image](https://user-images.githubusercontent.com/97303986/215501065-3e046d87-5a4b-4112-b600-7a21c6165ee1.png)

 

### prog_power_select

- Jumper is used for power routing during programming
- Cut trace to main and solder USB to center to enable USB power during programming.
- Ensure to remove USB side and replace main for normal use

## Circuit Snippets
_For future reference and reuse_

### Reverse Voltage Protection & Power Input
![image](https://user-images.githubusercontent.com/97303986/234007162-796d24b9-31ba-4529-b41d-d53ad71e6333.png)


### 5v Buck Converter
![image](https://user-images.githubusercontent.com/97303986/233372301-b49ece21-e5c7-4770-9f9d-a921e56cfa48.png)

### Current Sense Circuit
![image](https://user-images.githubusercontent.com/97303986/234006873-5b099b90-caab-46b2-af19-8a54f1b18855.png)

### DC/Dc Module
![image](https://user-images.githubusercontent.com/97303986/234007559-b9829580-6ffb-4fe2-b3de-4b5e0169443b.png)

### Top Level
![image](https://user-images.githubusercontent.com/97303986/234019618-974cba4d-d7e9-4111-9740-9a07acf87d8b.png)


## Net Classes
_Lots of attention was paid to Net Class definition and assignment for this project. It would be sensible to reuse these definitions and update if nessisary rather than start from scratch_

![image](https://user-images.githubusercontent.com/97303986/234025952-47013231-ef54-4bf2-926b-c18c8e58bd59.png)

![image](https://user-images.githubusercontent.com/97303986/234026151-1d6064d5-2849-49ab-87d3-ae31882a1986.png)

#### Schematic
Default	0.1524 mm	0.3048 mm	rgba(0, 0, 0, 0.000)	Solid
12V_BUS	0.1524 mm	0.3048 mm	rgb(214, 128, 31)	Solid
24V_BUS	0.1524 mm	0.3048 mm	rgb(200, 31, 33)	Solid
5V_BUS	0.1524 mm	0.3048 mm	rgb(193, 182, 20)	Solid
ANALOG	0.1524 mm	0.3048 mm	rgb(255, 49, 178)	Solid
CURRENT_SENSOR	0.1524 mm	0.3048 mm	rgb(80, 84, 255)	Solid
DIGITAL	0.1524 mm	0.3048 mm	rgb(168, 72, 185)	Solid
DIGITAL_GND	0.1524 mm	0.3048 mm	rgb(95, 91, 94)	Solid
GND	0.1524 mm	0.3048 mm	rgb(108, 79, 1)	Solid
MCU_5V_BUS	0.1524 mm	0.3048 mm	rgb(155, 222, 16)	Solid
MID_PWR_BUS	0.1524 mm	0.3048 mm	rgb(255, 255, 32)	Solid
PWR_GND	0.1524 mm	0.3048 mm	rgb(188, 29, 36)	Solid
PWR_OUTPUT	0.1524 mm	0.3048 mm	rgb(176, 255, 20)	Solid
USB_PBUS	0.1524 mm	0.3048 mm	rgb(52, 217, 159)	Solid

#### PCB
Default	0.2 mm	0.2 mm	0.8 mm	0.4 mm	0.3 mm	0.1 mm	0.2 mm	0.25 mm	
12V_BUS	0.1985 mm	6.5 mm	0.8 mm	0.4 mm	0.3 mm	0.1 mm	0.2 mm	0.25 mm	
24V_BUS	0.2 mm	4 mm	0.8 mm	0.4 mm	0.3 mm	0.1 mm	0.2 mm	0.25 mm	
5V_BUS	0.2 mm	4.5 mm	0.8 mm	0.4 mm	0.3 mm	0.1 mm	0.2 mm	0.25 mm	
ANALOG	0.2 mm	0.2 mm	0.8 mm	0.4 mm	0.3 mm	0.1 mm	0.2 mm	0.25 mm	
CURRENT_SENSOR	0.2 mm	7 mm	0.8 mm	0.4 mm	0.3 mm	0.1 mm	0.2 mm	0.25 mm	
DIGITAL	0.2 mm	0.2 mm	0.8 mm	0.4 mm	0.3 mm	0.1 mm	0.2 mm	0.25 mm	
DIGITAL_GND	0.2 mm	0.3 mm	0.8 mm	0.4 mm	0.3 mm	0.1 mm	0.2 mm	0.25 mm	
GND	0.2 mm	1.5 mm	0.8 mm	0.4 mm	0.3 mm	0.1 mm	0.2 mm	0.25 mm	
MCU_5V_BUS	0.2 mm	0.3 mm	0.8 mm	0.4 mm	0.3 mm	0.1 mm	0.2 mm	0.25 mm	
MID_PWR_BUS	0.2 mm	3 mm	0.8 mm	0.4 mm	0.3 mm	0.1 mm	0.2 mm	0.25 mm	
PWR_GND	0.1985 mm	7 mm	0.8 mm	0.4 mm	0.3 mm	0.1 mm	0.2 mm	0.25 mm	
PWR_OUTPUT	0.2 mm	2 mm	0.8 mm	0.4 mm	0.3 mm	0.1 mm	0.2 mm	0.25 mm	
USB_PBUS	0.2 mm	0.3 mm	0.8 mm	0.4 mm	0.3 mm	0.1 mm	0.2 mm	0.25 mm	




## Issues V1.0

1. Tx & Rx Pin swapped on CH340 - aTmeGA328P
 - To enable USB communication, reverse pins 2 & 3
