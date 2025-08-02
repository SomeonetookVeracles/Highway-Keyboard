I'm building a minimalistic keyboard, something simple and stripped down. It's my first time working on a large PCB, and I kept getting distracted by feature creep and add-ons. So I'm going back to basics. I want this to be a barebones board that helps me sharpen my skills and really dial in the core of what makes a great keyboard.

I learned a lot while doing this, and explored concepts like impedence matching and zones, something that I've done before but never really had to prioritize.

If I do this again, I'm using a ESP-32 chip, making a CPU clock with decoupling capacitors was exhausting and annoyed me to no small extent lmao.
<img width="1263" height="755" alt="473670760-d07d10b8-821d-4425-aa78-196647b4c1dc" src="https://github.com/user-attachments/assets/5ed16ddb-e6de-427f-978d-52f61724bdfb" />

<img width="1049" height="467" alt="image" src="https://github.com/user-attachments/assets/dda2eae3-8b45-42fc-9991-732e67c4005d" />

<img width="1308" height="519" alt="image" src="https://github.com/user-attachments/assets/279ececc-5a16-45be-bfb0-c403b565ecc9" />

# Bill of Materials

| Reference | Qty | Value | Footprint | Description | DigiKey Link | Amazon Link | Unit Price | Total Price |
|-----------|-----|-------|-----------|-------------|--------------|-------------|------------|-------------|
| **Capacitors** | | | | | | | | |
| C1 | 1 | 1uF | 0603 | Ceramic Capacitor | [YAGEO CC0603ZRY5V7BB105](https://www.digikey.com/en/products/detail/yageo/CC0603ZRY5V7BB105/2103110) | [0603 Capacitor Kit](https://www.amazon.com/100pcs-Multilayer-Ceramic-Capacitor-0-5pF/dp/B0DDC637G1) | $0.03 | $0.03 |
| C2,C3,C4 | 3 | 0.1uF | 0603 | Ceramic Capacitor | [KEMET C0603C104J4RAC7867](https://www.digikey.com/en/products/detail/kemet/C0603C104J4RAC7867/411096) | [0603 Capacitor Kit](https://www.amazon.com/100pcs-Multilayer-Ceramic-Capacitor-0-5pF/dp/B0DDC637G1) | $0.02 | $0.06 |
| C5 | 1 | 10uF | 0603 | Ceramic Capacitor | [YAGEO CC0603KRX5R6BB106](https://www.digikey.com/en/products/detail/yageo/CC0603KRX5R6BB106/5195191) | [0603 Capacitor Kit](https://www.amazon.com/100pcs-Multilayer-Ceramic-Capacitor-0-5pF/dp/B0DDC637G1) | $0.08 | $0.08 |
| C6,C7 | 2 | 22pF | 0603 | Ceramic Capacitor | [DigiKey 0603 Capacitors](https://www.digikey.com/en/products/filter/ceramic-capacitors/60) | [0603 Capacitor Kit](https://www.amazon.com/100pcs-Multilayer-Ceramic-Capacitor-0-5pF/dp/B0DDC637G1) | $0.02 | $0.04 |
| **Diodes** | | | | | | | | |
| D1-D87 | 87 | D_Small | 0603 | Small Signal Diode | [DigiKey 0603 Diodes](https://www.digikey.com/en/products/filter/diodes-rectifiers-single/280) | [SMD Component Kit](https://www.amazon.com/Component-Assortment-Capacitor-Transistor-Soldering/dp/B07GMRJC1Q) | $0.05 | $4.35 |
| **Fuse** | | | | | | | | |
| F1 | 1 | 500mA | 1812 | PTC Resettable Fuse | [Bourns MF-MSMF050-2](https://www.digikey.com/en/products/detail/bourns-inc/MF-MSMF050-2/662832) | [Fuse Kit](https://www.amazon.com/s?k=500mA+PTC+fuse) | $0.32 | $0.32 |
| **Connectors** | | | | | | | | |
| J1 | 1 | USB_C_Receptacle | HRO TYPE-C-31-M-12 | USB-C 2.0 Connector | [JAE DX07S016JA3R1500](https://www.digikey.com/en/products/detail/jae-electronics/DX07S016JA3R1500/5978550) | [USB-C Connector](https://www.amazon.com/s?k=TYPE-C-31-M-12) | $0.38 | $0.38 |
| **Resistors** | | | | | | | | |
| R1,R4 | 2 | 10k | 0603 | Chip Resistor | [YAGEO RC0603JR-0710KL](https://www.digikey.com/en/products/detail/yageo/RC0603JR-0710KL/726700) | [0603 Resistor Kit](https://www.amazon.com/s?k=0603+resistor+kit) | $0.01 | $0.02 |
| R2,R3 | 2 | 22Ω | 0603 | Chip Resistor | [DigiKey 0603 Resistors](https://www.digikey.com/en/products/filter/resistors/chip-resistor-surface-mount/0603/52) | [0603 Resistor Kit](https://www.amazon.com/s?k=0603+resistor+kit) | $0.01 | $0.02 |
| R5 | 1 | 1M | 0603 | Chip Resistor | [DigiKey 0603 Resistors](https://www.digikey.com/en/products/filter/resistors/chip-resistor-surface-mount/0603/52) | [0603 Resistor Kit](https://www.amazon.com/s?k=0603+resistor+kit) | $0.01 | $0.01 |
| R6,R7 | 2 | 5.11k | 0603 | Chip Resistor | [DigiKey 0603 Resistors](https://www.digikey.com/en/products/filter/resistors/chip-resistor-surface-mount/0603/52) | [0603 Resistor Kit](https://www.amazon.com/s?k=0603+resistor+kit) | $0.01 | $0.02 |
| **Switches** | | | | | | | | |
| SW1-SW87 | 87 | SW_Push_45deg | Cherry MX Compatible | Mechanical Key Switch | [Cherry MX1A-E1NW](https://www.digikey.com/en/products/detail/cherry-americas-llc/MX1A-E1NW/20180) | [Cherry MX Switches](https://www.amazon.com/s?k=cherry+mx+switches) | $1.25 | $108.75 |
| SWRST1 | 1 | SW_PUSH | SMD Tactile | Reset Switch | [DigiKey Tactile Switches](https://www.digikey.com/en/products/filter/tactile-switches/197) | [Tactile Switch Kit](https://www.amazon.com/s?k=SMD+tactile+switch) | $0.15 | $0.15 |
| **Microcontroller** | | | | | | | | |
| U1 | 1 | ATmega32U4-A | TQFP-44 | 8-bit Microcontroller | [ATMEGA32U4-AU](https://www.digikey.com/en/products/detail/microchip-technology/ATMEGA32U4-AU/1914602) | [ATmega32U4 Module](https://www.amazon.com/s?k=atmega32u4) | $5.39 | $5.39 |
| **Crystal** | | | | | | | | |
| Y1 | 1 | 16MHz | 0603-4Pin | Crystal Oscillator | [TXC 7V-16.000MAAE-T](https://www.digikey.com/en/products/detail/txc-corporation/7V-16-000MAAE-T/2626978) | [16MHz Crystal](https://www.amazon.com/s?k=16MHz+crystal+SMD) | $0.35 | $0.35 |
