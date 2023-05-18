# Hacking the Incubator

One of our lab incubators is a relatively cheap (¥10,000 - ¥15,000) incubator, that can both heat & cool. It has a peltier device, a temp sensor, a fan for internal circulation and a fan to cool the peltier.
It's controlled by 4 buttons on the front (power, temp up, temp down, light).

You can get one from [here](https://www.amazon.co.jp/-/en/VS-404-Versos-25L-Portable-Pack/dp/B00ADEHRL8/).

`34.5D x 43W x 48.5H cm`
`25 Liters`

## Disassembly

We decided to open the incubator up and see how its made.

### Back Panel
![](https://github.com/BioClub/Incubator/blob/main/images/power/DSC_4187.JPG)
Opening up the Incubator

![](https://github.com/BioClub/Incubator/blob/main/images/power/DSC_4192.JPG)

![](https://github.com/BioClub/Incubator/blob/main/images/power/DSC_4193.JPG)
Power Board

![](https://github.com/BioClub/Incubator/blob/main/images/power/DSC_4207.JPG)
The Peltier Device is connected to a heat sink inside the incubator

![](https://github.com/BioClub/Incubator/blob/main/images/power/DSC_4208.JPG)
The Peltier Device is connected to a heat sink inside the incubator

![](https://github.com/BioClub/Incubator/blob/main/images/power/DSC_4204.JPG)
Temperature Sensor & Circulation Fan

### Front Panel

![](https://github.com/BioClub/Incubator/blob/main/images/front/Incubator_Panel.jpg)
Openend Front Panel

- Power Push Button, with 4 LEDs for visual feedback
- U1: [78D05L](https://github.com/BioClub/Incubator/blob/main/datasheets/78DXXL.pdf), 5V 0.5A Voltage Regulator
- U2: Unspecified MCU, Maybe a [PIC16](https://github.com/BioClub/Incubator/blob/main/datasheets/30277d.pdf)?
- U3: [74HC164D](https://github.com/BioClub/Incubator/blob/main/datasheets/74HC164D.pdf), 8-Bit Shift Register for driving Segment LCD Display

Clearly visible is also the 5 pin connector for the ISP.

![](https://github.com/BioClub/Incubator/blob/main/images/front/LogicBoard_Details.jpg)

![](https://github.com/BioClub/Incubator/blob/main/images/front/Front_Panels_Removed_123.jpg)



