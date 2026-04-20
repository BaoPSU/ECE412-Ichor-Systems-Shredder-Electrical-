# Hardware Components

## PLC System
| Component | Model | Notes |
|---|---|---|
| PLC Rack | DirectLOGIC 205 D2-09B-1 | 9-slot base unit |
| CPU | H2-DM1E | Built-in Ethernet, executes ladder logic |
| Discrete Input | D2-08ND3 | 8-ch 24VDC digital inputs (Slot 2) |
| Analog Input | F2-06AD-1 | 6-ch 4–20mA / 0–10V (Slot 3) |
| RTD Input | F2-04RTD | 4-ch PT100/PT1000 temp (Slot 4) |
| Discrete Output | D2-08TD2 | 8-ch 12–24VDC transistor sourcing (Slot 5) |
| Analog Output | F2-02DAS-2 | 2-ch 4–20mA / 0–10V (Slot 6) |
| Fill Panels | D2-Fill | Slots 7, 8, 9 (reserved) |

## HMI
| Component | Model | Notes |
|---|---|---|
| Touch Panel | EA9-T6CL-R | 6" C-More color touch panel |
| HMI Power Supply | Rhino PSB12-030-P | DC supply for HMI |
| PLC–HMI Link | Serial (COM port) | Match baud/parity/stop bits on both ends |

## Power
| Component | Model | Notes |
|---|---|---|
| 24VDC Power Supply | Mean Well NDR-480-24 | Powers PLC I/O, contactor coil, pushbutton commons |
| Fuse Block (main) | MORSETTITALIA EURO S10H-5H | 25A for PSU branch, 1A for PLC branch |
| Pushbutton fuse | MORSETTITALIA EURO S4LH | 1.5A fast blow, distributed to pushbutton commons |

## Motor Control
| Component | Model | Notes |
|---|---|---|
| VFD | HY Series HY02D211B-T | Receives 0–10V speed command via analog output CH1 |
| Contactor | Mitsubishi SD-N35 | Coil driven by D2-08TD2 Y0 output (+24VDC) |
| Motor Overload | Phoenix Contact TMC 83C 15A (2907618) | AC line protection before contactor |
| Thermal Overload | RTD32-180 | NC contact feeds F2 coil; driven by OUT3 |

## Safety / Control
| Component | Notes |
|---|---|
| E-stop | Hardwired NC into safety circuit |
| Two-hand start | Forward + Deadman SW1 + Deadman SW2 buttons (24VDC, fused 1.5A) |
| Lid interlock | DI input to PLC |
| Status lights | Power on / Running / Fault (driven by discrete outputs) |

## Wiring Accessories
| Component | Model | Notes |
|---|---|---|
| ZipLink Terminal Block | ZL-RTB20-OUT | Output module field wiring interface |
| ZipLink Terminal Block | ZL-RTB20 | Analog output field wiring interface |
| Contactor fuse | DF103V 1/2A slow blow | Protects D2-08TD2 output to contactor coil A1 |
