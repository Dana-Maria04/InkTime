# InkTime

## Block Diagram

Managed by the nRF52840 SoC, the device employs an RT6160 regulator to provide a steady 3.3V supply to all peripherals. The architecture combines an e-paper display and IMU with haptic feedback and dedicated user buttons.

<img width="1230" height="814" alt="Diagrama" src="https://github.com/user-attachments/assets/d5b46a55-2d0a-4a43-bef1-5201cc3a067a" />


## Bill of Materials (BOM)
| Qty | Value             | Parts                                                                     | Device                              | Package                      | Product Link                                                                        | Datasheet Link                                                                                                                                   |
| --: | ----------------- | ------------------------------------------------------------------------- | ----------------------------------- | ---------------------------- | ----------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------ |
|   1 | nRF52840-QIAA     | U1                                                                        | NORDIC_NRF_4_NRF52840_QF            | AQFN-73-EP(7x7)              | [JLCPCB](https://jlcpcb.com/partdetail/NordicSemicon-NRF52840_QIAAR/C190794)        | [Datasheet](https://infocenter.nordicsemi.com/pdf/nRF52840_PS_v1.9.pdf)                                                                          |
|   1 | BQ25180YBGR       | IC1                                                                       | BQ25180YBGR                         | DSBGA-8(1.1x1.6)             | [JLCPCB](https://jlcpcb.com/partdetail/TexasInstruments-BQ25180YBGR/C3682423)       | [Datasheet](https://www.ti.com/lit/ds/symlink/bq25180.pdf)                                                                                       |
|   1 | MAX17048G+T10     | U3                                                                        | ESP32_C6_LIBRARY_MAX17048G+T10      | DFN-8-EP(2x2)                | [JLCPCB](https://jlcpcb.com/partdetail/MaximIntegrated-MAX17048GT10/C2682616)       | [Datasheet](https://www.analog.com/media/en/technical-documentation/data-sheets/MAX17048-MAX17049.pdf)                                           |
|   1 | DRV2605YZFR       | IC2                                                                       | DRV2605YZFR                         | DSBGA-9                      | [JLCPCB](https://jlcpcb.com/partdetail/TexasInstruments-DRV2605YZFR/C81079)         | [Datasheet](https://www.ti.com/lit/ds/symlink/drv2605.pdf)                                                                                       |
|   1 | DMG2305UX-7       | P-channel MOSFET                                                          | DMG2305UX-7                         | SOT-23                       | [JLCPCB](https://jlcpcb.com/partdetail/HXYMOSFET-DMG2305UX7/C5261054)               | [Datasheet](https://www.diodes.com/assets/Datasheets/DMG2305UX.pdf)                                                                              |
|   1 | SI1308EDL-T1-GE3  | Q3                                                                        | ESP32_C6_LIBRARY_6_SI1308EDL-T1-GE3 | SOT-323                      | [JLCPCB](https://jlcpcb.com/partdetail/TECHPUBLIC-SI1308EDL/C7603347)               | [Datasheet](https://www.vishay.com/docs/63399/si1308edl.pdf)                                                                                     |
|   3 | MBR0530           | D2, D4, D5                                                                | MBR0530                             | SOD-123                      | [JLCPCB](https://jlcpcb.com/partdetail/4324765-MBR0530_F20000HF/C3757235)           | [Datasheet](https://wmsc.lcsc.com/wmsc/upload/file/pdf/v2/lcsc/2205311800_Yangzhou-Yangjie-Electronic-Technology-MBR0530-F2-0000HF_C3757235.pdf) |
|   1 | USBLC6-2SC6Y      | D3                                                                        | USBLC6-2SC6Y                        | SOT-23-6                     | [JLCPCB](https://jlcpcb.com/partdetail/TECHPUBLIC-USBLC62SC6Y/C5310974)             | [Datasheet](https://wmsc.lcsc.com/wmsc/upload/file/pdf/v2/lcsc/2401261525_TECH-PUBLIC-USBLC6-2SC6Y_C5310974.pdf)                                 |
|   1 | 2450AT18B100E     | ANT1                                                                      | 2450AT18B100E_2450AT18B100E         | ANTC3216X140N / 1206 class   | [JLCPCB](https://jlcpcb.com/partdetail/JohansonTechnology-2450AT18B100/C2836414)    | [Datasheet](https://www.johansontechnology.com/datasheets/antennas/2450AT18B100.pdf)                                                             |
|   1 | KH-TYPE-C-16P     | J4                                                                        | KH-TYPE-C-16P_KH-TYPE-C-16P         | SMD                          | [JLCPCB](https://jlcpcb.com/partdetail/KH-TYPE-C-16P/C709357)                       | [Datasheet](https://wmsc.lcsc.com/wmsc/upload/file/pdf/v2/lcsc/2204251630_SHENZHEN-KINGHELM-Elec-KH-TYPE-C-16P_C709357.pdf)                      |
|   3 | EVP-AKE31A        | SW_DN, SW_ENT, SW_UP                                                      | EVP-AKE31A                          | SW_EVP-AKE31A_PAN            | [JLCPCB](https://jlcpcb.com/partdetail/PANASONIC-EVPAKE31A/C569760)                 | [Datasheet](https://www.lcsc.com/datasheet/C569760.pdf)                                                                                          |
|   1 | FTC252012SR47MBCA | L7                                                                        | MLP2016SR47MT0S1_FTC252012SR47MBCA  | INDC2016X100N                | [JLCPCB](https://jlcpcb.com/partdetail/6763488-FTC252012SR47MBCA/C5832368)          | [Datasheet](https://wmsc.lcsc.com/wmsc/upload/file/pdf/v2/lcsc/2311271530_TDK-FTC252012SR47MBCA_C5832368.pdf)                                    |
|   1 | 32.768 kHz        | X2                                                                        | NORDIC_NRF_1_XTAL_32KHZ             | SMD3215-2P                   | [JLCPCB](https://jlcpcb.com/partdetail/NDK-NX3215SA_32_768K_STD_MUA9/C519280)       | [Datasheet](https://www.ndk.com/images/products/crystal/resonator/NX3215SA_e.pdf)                                                                |
|   6 | 10K               | R2_EP_DR, R5, R7, R8, R9, R_PWR_EPD                                       | RC0201FR-1310KL                     | 0201                         | [JLCPCB](https://jlcpcb.com/partdetail/YAGEO-RC0201FR1310KL/C6373588)               | [Datasheet](https://www.lcsc.com/datasheet/C6373588.pdf)                                                                                         |
|   2 | 5K1               | R1_USB, R2_USB                                                            | RC0201FR-075K1L                     | 0201                         | [JLCPCB](https://jlcpcb.com/partdetail/YAGEO-RC0201FR075K1L/C274341)                | [Datasheet](https://www.lcsc.com/datasheet/C274341.pdf)                                                                                          |
|   2 | 3K3               | R17, R18                                                                  | RNCF0201DTC3K30                     | 0201                         | [JLCPCB](https://jlcpcb.com/partdetail/SEI_Stackpole_Elec-RNCF0201DTC3K30/C2487997) | [Datasheet](https://www.lcsc.com/datasheet/C2487997.pdf)                                                                                         |
|   3 | 0R                | R2, R3, R4                                                                | 0201WMJ0000TCE                      | 0201                         | [JLCPCB](https://jlcpcb.com/partdetail/25793-0201WMJ0000TCE/C25050)                 | [Datasheet](https://www.lcsc.com/datasheet/C25050.pdf)                                                                                           |
|   1 | 2.2Î©              | R_TYPE_SEL                                                                | 0201WMF220KTCE                      | 0201                         | [JLCPCB](https://jlcpcb.com/partdetail/244650-0201WMF220KTCE/C247442)               | [Datasheet](https://www.lcsc.com/datasheet/C247442.pdf)                                                                                          |
|   9 | 100nF             | C5, C7, C8, C12, C19, C23, C27, C34, C42                                  | AC0201KRX6S6BB104                   | 0201                         | [JLCPCB](https://jlcpcb.com/partdetail/YAGEO-AC0201KRX6S6BB104/C3855913)            | [Datasheet](https://www.lcsc.com/datasheet/C3855913.pdf)                                                                                         |
|   4 | 12pF              | C1, C2, C17, C18                                                          | 0201N120J250CT                      | 0201                         | [JLCPCB](https://jlcpcb.com/partdetail/Walsin_TechCorp-0201N120J250CT/C424835)      | [Datasheet](https://www.lcsc.com/datasheet/C424835.pdf)                                                                                          |
|   2 | 1pF               | C3, C4                                                                    | GRM0335C1E1R0CA01J                  | 0201                         | [JLCPCB](https://jlcpcb.com/partdetail/2274979-GRM0335C1E1R0CA01J/C2182912)         | [Datasheet](https://www.lcsc.com/datasheet/C2182912.pdf)                                                                                         |
|   1 | 100pF             | C11                                                                       | 0201N101F160CT                      | 0201                         | [JLCPCB](https://jlcpcb.com/partdetail/Walsin_TechCorp-0201N101F160CT/C3847857)     | [Datasheet](https://www.lcsc.com/datasheet/C3847857.pdf)                                                                                         |
|   1 | 47nF              | C16                                                                       | C0201X5R473K160NTA                  | 0201                         | [JLCPCB](https://jlcpcb.com/partdetail/126083-C0201X5R473K160NTA/C124806)           | [Datasheet](https://www.lcsc.com/datasheet/C124806.pdf)                                                                                          |
|   1 | 1uF               | C15                                                                       | CL05A105KP5NNNC                     | 0402                         | [JLCPCB](https://jlcpcb.com/partdetail/C14445)                                      | [Datasheet](https://www.lcsc.com/datasheet/C14445.pdf)                                                                                           |
|   5 | 4.7uF             | C6, C14, C20, C21, C43                                                    | GRM155R61A475KEAAD                  | 0402                         | [JLCPCB](https://jlcpcb.com/partdetail/MurataElectronics-GRM155R61A475KEAAD/C77004) | [Datasheet](https://www.lcsc.com/datasheet/C77004.pdf)                                                                                           |
|   1 | 4.7uF / 25V       | C2-EP-DR                                                                  | C0402X5R475M250NT                   | 0402                         | [JLCPCB](https://jlcpcb.com/partdetail/SANYEAR-C0402X5R475M250NT/C2911388)          | [Datasheet](https://www.lcsc.com/datasheet/C2911388.pdf)                                                                                         |
|   9 | 1uF / 50V         | EPD_C1, EPD_C2, EPD_C6, EPD_C7, EPD_C8, EPD_C9, EPD_C10, EPD_C11, EPD_C12 | GRM155R61H105KE05D                  | 0402                         | [JLCPCB](https://jlcpcb.com/partdetail/1609005-GRM155R61H105KE05D/C1518208)         | [Datasheet](https://www.lcsc.com/datasheet/C1518208.pdf)                                                                                         |
|   2 | 10uF              | C24, C39                                                                  | 0402X106M100CT                      | 0402                         | [JLCPCB](https://jlcpcb.com/partdetail/Walsin_TechCorp-0402X106M100CT/C2992625)     | [Datasheet](https://www.lcsc.com/datasheet/C2992625.pdf)                                                                                         |
|   2 | 22uF              | C25, C33                                                                  | CL05A226MQ6ZUN8                     | 0402                         | [JLCPCB](https://jlcpcb.com/partdetail/2889851-CL05A226MQ6ZUN8/C2762589)            | [Datasheet](https://www.lcsc.com/datasheet/C2762589.pdf)                                                                                         |
|   1 | 820pF             | C9                                                                        | MA0201XF821K250                     | 0201                         | [JLCPCB](https://jlcpcb.com/partdetail/Meritek-MA0201XF821K250/C3842403)            | [Datasheet](https://www.lcsc.com/datasheet/C3842403.pdf)                                                                                         |
|   1 | 32MHz             | X1                                                                        | NX2016SA-32MHZ-STD-CZS-5            | SMD2016-4P                   | [JLCPCB](https://jlcpcb.com/partdetail/NDK-NX2016SA_32MHZ_STD_CZS5/C843260)         | [Datasheet](https://www.lcsc.com/datasheet/C843260.pdf)                                                                                          |
|   1 | 3.9nH             | L1                                                                        | VHF060303H3N9ST                     | 0201                         | [JLCPCB](https://jlcpcb.com/partdetail/153834-VHF060303H3N9ST/C142503)              | [Datasheet](https://www.lcsc.com/datasheet/C142503.pdf)                                                                                          |
|   1 | 15nH              | L3                                                                        | MLK0603L15NJT000                    | 0201                         | [JLCPCB](https://jlcpcb.com/partdetail/TDK-MLK0603L15NJT000/C6990407)               | [Datasheet](https://www.lcsc.com/datasheet/C6990407.pdf)                                                                                         |
|   1 | BMA421            | IC3                                                                       | BMA421                              | LGA-12(2x2)                  | [JLCPCB](https://jlcpcb.com/partdetail/BoschSensortec-BMA421/C5242966)              | [Datasheet](https://files.pine64.org/doc/datasheet/pinetime/BST-BMA421-FL000.pdf)                                                                |
|   1 | RT6160AWSC        | IC9                                                                       | RT6160AWSC                          | WLCSP-15B(2.3x1.4)           | [JLCPCB](https://jlcpcb.com/partdetail/RichtekTech-RT6160AWSC/C7065276)             | [Datasheet](https://www.mouser.com/datasheet/2/1458/DS6160A_03-3104604.pdf)                                                                      |
|   1 | 503480-2400       | J1                                                                        | 5034802400                          | 24-pin 0.5mm right-angle FPC | [JLCPCB](https://jlcpcb.com/partdetail/MOLEX-5034802400/C122434)                    | [Datasheet](https://www.mouser.com/datasheet/2/276/2/5034802400_FFC_FPC_CONNECTORS-1112921.pdf)                                                  |

## System Design and Hardware Implementation

The hardware architecture of the **InkTime Smartwatch** centers on the **nRF52840 microcontroller**, integrating five specialized sub-systems to create a high-efficiency wearable device.

### 1. Central SoC & Communication
The **nRF52840** handles all high-level logic, from sensor fusion to Bluetooth LE communication. It utilizes a **32 MHz crystal** for active processing and a **32.768 kHz crystal** for low-power timekeeping. For debugging and firmware updates, a **TC2030 SWD header** is included, exposing the `SWDIO` and `SWDCLK` lines.

### 2. Power Subsystem & Efficiency
Energy is managed through a multi-stage architecture:
* **USB-C Input:** Protected by **USBLC6-2SC6Y** ESD diodes to ensure safety during charging.
* **Management:** The **BQ25180 charger** regulates power flow between the USB source and the **Li-Po battery**.
* **Efficiency:** An **RT6160 Buck-Boost converter** ensures all peripherals receive exactly **3.3V**, regardless of battery discharge levels.
* **Monitoring:** The **MAX17048 fuel gauge** uses I2C to alert the MCU of low-battery conditions in real-time.

### 3. Specialized Sub-systems
* **Display:** The **1.54-inch E-Ink panel** uses an SPI interface. Its bi-stable nature allows it to hold an image without consuming power, drastically reducing the overall energy profile.
* **Motion & Interaction:** An **IMU (BMA421/423)** monitors activity, while three GPIO-mapped buttons manage user navigation and input.
* **Haptics:** Physical feedback for notifications is provided by a vibration motor controlled by the **DRV2605 driver**, which supports pre-programmed haptic patterns over I2C.

### 4. Energy Estimation
The system is optimized for an extremely low duty cycle:
* **Deep Sleep:** $< 10\text{µ}$.
* **Active Refresh:** $8\text{-}10\text{ mA}$ for approximately $1\text{-}2$ seconds per minute.

Based on the **250 mAh** battery capacity, the smartwatch achieves an autonomy of **over 9 days**, even with active sensor monitoring and daily haptic notifications. This performance highlights the synergy between the E-Ink technology and the nRF52's advanced power-saving features.

### Detailed Pinnout Map of nRF52840

| nRF52840 Pin | Connected Block | Signal Name | Purpose / Function |
| :--- | :--- | :--- | :--- |
| **P1.13** | E-paper Display | `MOSI` | SPI data output to display |
| **P1.15** | E-paper Display | `SCK` | SPI serial clock line |
| **P0.05** | E-paper Display | `EPD_CS` | SPI chip select (active low) |
| **P0.16** | E-paper Display | `EPD_DC` | Data/Command selection toggle |
| **P0.17** | E-paper Display | `EPD_RST` | Hardware reset for display |
| **P0.15** | E-paper Display | `EPD_BUSY` | Status feedback (busy/ready) |
| **P0.06** | I2C Bus (Shared) | `SDA` | Data line for IMU, Fuel Gauge, and Haptic |
| **P0.07** | I2C Bus (Shared) | `SCL` | Clock line for IMU, Fuel Gauge, and Haptic |
| **P0.08** | IMU (BMA42x) | `IMU_INT1` | Primary motion interrupt |
| **P1.08** | IMU (BMA42x) | `IMU_INT2` | Secondary motion interrupt |
| **P0.11** | PMIC (BQ25180) | `PMIC_INT` | Power-management status interrupt |
| **P0.24** | Fuel Gauge | `ALERT` | Battery fuel gauge status alert |
| **P0.12** | Haptic Driver | `HAPTIC_EN` | Enable and control for DRV2605 |
| **P0.13** | USB-C Interface | `D+` | USB differential data positive |
| **P0.14** | USB-C Interface | `D-` | USB differential data negative |
| **VBUS pin** | Charger / USB-C | `VBUS` | USB voltage presence detection |
| **SWDIO** | SWD Header | `SWDIO` | Bidirectional debug/programming data |
| **SWDCLK** | SWD Header | `SWDCLK` | Debug/programming clock reference |
| **P1.09** | SWD Header | `SWO` | Single Wire Output (trace debug) |
| **P0.18 / RESET** | SWD Header | `RESET` | Global hardware reset line |
| **ANT pin** | RF Network | `RF` | 2.4 GHz connection to chip antenna |


## Design Decisions & DRC/ERC Notes

### 1. Hardware Design Log
* **Space Optimization:** To fit the enclosure, a **1.0 mm PCB** was used with all components mounted on the **TOP layer**. The use of **0201 footprints** was critical for the high-density layout.
* **Signal Integrity:** **100 nF decoupling capacitors** are placed as close as possible ($< 0.5$ mm) to power pins. Power traces are widened to **0.3 mm** to ensure stable voltage delivery.
* **RF Layout:** The antenna is positioned on the board edge with a clear **Keep-out zone** (no copper on any layer) to maximize Bluetooth connectivity.

### 2. Validation & Manual Approvals
The following CAD warnings were reviewed and approved based on project constraints:

* **Mechanical Alignment (DRC):** Dimension errors for the **USB-C connector and tactile buttons** were ignored because their placement must match the pre-defined enclosure openings.
* **High-Density Routing (DRC):** Overlaps caused by **via-in-pad** and escape routing for the nRF52840 were accepted. This was the only way to route the MCU pins in the available space.
* **Net Connectivity (ERC):** "Only INPUT pins" warnings were verified; the schematic is functionally complete, and these are typical false positives in this project context.
* **Power Pins (ERC):** Power rail warnings were manually checked to ensure that the **RT6160** and **BQ25180** correctly supply the 3.3V and VBAT nets.
