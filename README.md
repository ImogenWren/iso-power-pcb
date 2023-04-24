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


## Issues V1.0

1. Tx & Rx Pin swapped on CH340 - aTmeGA328P
 - To enable USB communication, reverse pins 2 & 3
