---
title: "Understanding USB"
author: "Henry Marshall"

separator: "^={4,}$"
separator-vertical: "^-{4,}$"
separator-notes: "^Notes?:"
charset: "utf-8"
---

# Understanding USB
## Why this cable works, and that one doesn't

<p style="text-align: center;">Henry Marshall</p>
<p style="text-align: center;">2019-03-11</p>

==========

## USB Spec

---------

## Not Just 1 Spec

----------

* Ports
* Data
* Charging

==========

## Ports

----------

![USB A 2.0 Upside Down](./images/usb_a_2_upside_down.png)

----------

## USB A

![USB A 2.0](./images/usb_a_2.jpg)

----------

## USB B

![USB B 2.0](./images/usb_b_2.png)

----------

## USB C

![USB C](./images/usb_c.png)

----------

## Micro USB

![Micro USB 2.0](./images/micro_2.jpg)

==========

## Data

----------

| Version         | Marketing Name           |
| --------------- | ------------------------ |
| USB 2.0         | High Speed  (480 Mbit/s) |
| USB 3.0         | SuperSpeed  (5Gbit/s)    |
| USB 3.1         | SuperSpeed+ (10 Gbit/s)  |
| USB 3.2         | SuperSpeed+ (20 Gbit/s)  |
| USB4 (upcoming) | SuperSpeed+ (40 Gbit/s)  |
| Thunderbolt 3   |                          |
| DisplayPort     |                          |

----------

| Version         | 2013-01       | 2017-07         |
| --------------- | ------------- | --------------- |
| USB 2.0         |               |                 |
| USB 3.0         | USB 3.1 Gen 1 | USB 3.2 Gen 1   |
| USB 3.1         | USB 3.1 Gen 2 | USB 3.2 Gen 2   |
| USB 3.2         |               | USB 3.2 Gen 2x2 |
| USB4 (upcoming) |               |                 |
| Thunderbolt 3   |               |                 |
| DisplayPort     |               |                 |

Note: I will use 3.0, 3.1, and 3.2

==========

## Where the Trouble Starts

----------

## Ports

| Version            | A     | B     | C     | Micro |
| ------------------ | ----- | ----- | ----- | ----- |
| USB 2.0            | ✅    | ✅    | ✅   | ✅    |
| USB 3.0            | ✅    | ✅    | ✅   | ✅    |
| USB 3.1            | ✅    | ✅    | ✅   | ✅    |
| USB 3.2            | ❌    | ❌    | ✅   | ❌    |
| USB4 (upcoming)    | ❌    | ❌    | ✅   | ❌    |
| Thunderbolt3 (TB3) | ❌    | ❌    | ✅   | ❌    |
| DisplayPort (DP)   | ❌    | ❌    | ✅   | ❌    |

----------

## USB A 3.x is Blue

![USB A 3.x](./images/usb_a_3.jpg)

----------

## USB B 3.x

![Micro 3](./images/micro_3.jpg)

----------

## Micro USB 3.x

![USB B 3](./images/usb_b_3.jpg)

----------

## USB C ???

![USB C](./images/usb_c.jpg)

Note:
- I wrap in elec tape
- MBP comes with 2.0

----------

![Unhelpful OEM](./images/unhelpful_oem.png)

Note: 
- This is getting better
- Pictured is [Samsung Notebook 9](https://www.samsung.com/us/computing/windows-laptops/notebook-series-9/notebook-9-15-led-full-hd-core-i7-np900x5l-k02us/#specs)

----------

## Thunderbolt 3

![Thunderbolt 3](./images/tb_3.jpg)

Note: 4 lane vs 2 lane

----------

## Ports

| Version            | A     | B     | C     | Micro |
| ------------------ | ----- | ----- | ----- | ----- |
| USB 2.0            | Black | Small | ???   | Small |
| USB 3.0            | Blue  | Big   | ???   | Big   |
| USB 3.1            | Blue  | Big   | ???   | Big   |
| USB 3.2            | x     | x     | ???   | x     |
| USB4 (upcoming)    | x     | x     | ???   | x     |
| Thunderbolt3 (TB3) | x     | x     | Bolt  | x     |
| DisplayPort (DP)   | x     | x     | ???   | x     |

==========

## Graceful Degredation

----------

## Lowest Common Denominator

- Host
- Peripheral
- Cable

Note: Cables can partially break

==========

## Why Protocols Matter

----------

## Speed

Note: Demo TB3 transfer & USB 2.0 Transfer + Magic Trick

----------

## Alt Mode DP Monitors

----------

## External GPU

==========

## Charging

----------

## Watt = Volt * Amp

Note: Watt is ultimately what matters

----------

## 10W = 5V * 2A

Note: Many chargers do not say `Watt` anywhere

----------

| Open Standard             | Maximum Power                |
| ------------------------- | ---------------------------- |
| USB 2.0                   | 2.5W = 5V at 0.5A            |
| USB 3.0                   | 4.5W = 5V at 0.9A            |
| Battery Charging v1.2     | 25W  = 5V at 5A (Typical 2A) |
| Power Delivery (PD)       | 100W = 5/9/15/20V at 5A      |

Note: 
- PD requires USB C
- HT to Google & Motorola for using PD

----------

| Proprietary Standard      | Maximum Power                 |
| ------------------------- | ----------------------------- |
| Quick Charge 1.0          | 10W = 5V at 2A                |
| Quick Charge 2.0          | 18W = 5/9/12V at 3A           |
| Quick Charge 3.0          | 18W = 3.6-20V at 2.5/4.6A     |
| Quick Charge 4.0+         | QC 3 & 27W PD (9V at 3A)      |
| Samsung AFC               | 18W = 5/9V at 1.67/2A         |
| One Plus WC 30            | 30W = 5V at 6A                |
| Huawei SC 2.0             | 40W = 5/9/10V at 2/4A         |
| Oppo VOOC 2               | 50W = 5V at 10A               |

Note: 
- Why do this? Predate PD & Very Fast
- All implement Battery Charging 1.2
- Samsung AFC ~== QC 2

----------

## Lowest Common Denominator

- Charger
- Device
- Cable

Note: Cable ~only relevant for 2A+

==========

## Maximizing your Speed

Note: First party best unless apple

----------

## Power Meter

==========

## Batteries

Note: 
- Why rapidly discharge at beginning
- Partial discharges are better for longevity
- Complete discharge to reset meter

----------

## Wireless Charging

![Qi Logo](./images/qi_logo.svg)

Note: 
- Wattage Matters
- Wireless less efficient
- Safer for public charging
- Samsung 15W; Apple 7.5W

==========

Assets

- [USB A 2.0](https://it.wikipedia.org/wiki/File:USB_Type-A_plug_coloured.svg)
- USB B 2.0 by [Edwin Javier Nuñez](https://commons.wikimedia.org/wiki/File:USB2HAB.jpg)

- USB A 2.0: Vahid alpha at [English Wikipedia](https://en.wikipedia.org/wiki/File:Usb_head_Cable.jpg)
- USB A 3.x: Rainer Knäpper, [Free Art License](http://artlibre.org/licence/lal/en/)
- Micro USB 3.0: Rainer Knäpper, [Free Art License](http://artlibre.org/licence/lal/en/)
- USB B 3.0: Anıl Öztaş
- USB C: Max Pixel
- USB C with Laptop: Maurizio Pesce
- Thunderbolt 3: Amin on [Wikimedia](https://commons.wikimedia.org/wiki/File:Thunderbolt_3_Cable_connected_to_OWC_Thunderbolt_3_Dock.jpg)

------------

## Questions