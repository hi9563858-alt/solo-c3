The Solo-C3 is a sleek, ultra-low-profile DIY smartwatch powered by the ESP32-C3 architecture. It features a streamlined, single-button media navigation menu, a 0.96-inch monochrome blue OLED display, local timekeeping synced via Bluetooth Low Energy (BLE), and an advanced power-management system utilizing deep sleep logic for maximum battery efficiency.
The custom internal hardware sandwich layout runs entirely pin-free on a flat 2-layer PCB and features external debugging pads alongside an integrated USB-C battery charging pipeline on the rear panel.

Key Features

Single-Button Media Control: Actively operates as a native HID consumer remote device. Control your smartphone's music loop over local Bluetooth using a multi-click pattern via the side-crown button (1 Click = Play/Pause, 2 Clicks = Next Track, 3 Clicks = Previous Track).

Deep Sleep Infrastructure: Enters a sub-1mA low-power sleep phase by completely disabling its internal Wi-Fi and Bluetooth radios while safely preserving local RTC time tracking. It awakens instantly via external GPIO interrupts.

Pinless Architecture: Engineered without structural header pins to enforce a flat, tight hardware enclosure profile under 12mm thickness.

Chassis Assembly: A rugged, modular 3-piece 3D-printed enclosure secured via 4 countersunk rear machine screws for simple hardware servicing and rapid battery swaps.

Bill of Materials (BOM)

1.Core Hardware & Semiconductor Layout

Microcontroller Module: ESP32-C3-MINI-1 System-on-Module (Integrated chip, oscillator, and PCB antenna block).

Display Panel: 0.96-inch Monochrome Blue OLED glass panel (128x64 pixels, driven via I2C interface).

Battery System: 3.7V Lithium-Polymer (LiPo) cell - Model 502035 (350mAh capacity, 5mm x 20mm x 35mm dimensions with an integrated PCM protection board) [350mAh].

Battery Socket Interface: Low-profile SMD 2-pin JST-SH connector (1.0mm pitch spacing).

2.Custom PCB Active Components

Voltage Regulator (LDO): XC6206P332MR Linear Regulator (SOT-23 package, regulates changing battery range smoothly down to a fixed 3.3V rail)

Battery Charging IC: TP4054 or TP4056 linear lithium management controller (manages 4.2V constant-voltage termination loop over USB input).

System Inputs: 1x Right-Angle Horizontal SMD tactile micro push-button (side-crown integration).

Charging Interface: 1x Mid-mount/Flush SMD USB-C receptacle (or exposed gold-plated pogo-pad terminals).

3.Structural Mechanics & Enclosure

Main Chassis: 3D-Printed Top Bezel and Baseplate (Filament recommendation: PETG or PLA for structural stiffness).

Wearable Strap: 3D-Printed flexible watch strap (Filament recommendation: TPU 95A rubberized filament) or standard 20mm universal watch fabric band.

Fasteners: 4x M2 Metric machine screws (4mm to 6mm length, flat countersunk head profiles).

*warning this is wip so some of this stuff will change be careful about which one you use*
