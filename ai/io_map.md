# PLC I/O Map — DirectLOGIC 205 D2-09B-1

## Rack Slot Layout
| Slot | Module | Type | Points |
|---|---|---|---|
| 1 | H2-DM1E | CPU / Ethernet | — |
| 2 | D2-08ND3 | 8-ch DI (24VDC) | X0–X7 |
| 3 | F2-06AD-1 | 6-ch AI (4–20mA / 0–10V) | — |
| 4 | F2-04RTD | 4-ch RTD input | — |
| 5 | D2-08TD2 | 8-ch DO (12–24VDC sourcing) | Y0–Y7 |
| 6 | F2-02DAS-2 | 2-ch AO (4–20mA / 0–10V) | — |
| 7–9 | D2-Fill | Reserved | — |

## Discrete Outputs (D2-08TD2, Slot 5)
| Address | Load | Notes |
|---|---|---|
| Y0 | Mitsubishi SD-N35 Contactor coil A1 | +24VDC via DF103V 1/2A fuse |

## Analog Output (F2-02DAS-2, Slot 6)
| Channel | Destination | Signal |
|---|---|---|
| CH1 | VFD HY02D211B-T terminal AL | 0–10V speed command via ZipLink ZL-RTB20 |

## Output Module — AC Relay (D2-08TA, separate)
| Address | Load | Notes |
|---|---|---|
| OUT0 | TX Contactor (GH15-BN) coil A1 | Via ZipLink, 120VAC common fused 1A slow blow |
| OUT1 | BUS Contactor (GH15-BN) coil A1 | Via ZipLink |
| OUT2 | F1 Contactor (GH15-BN) coil A1 | Via ZipLink |
| OUT3 | Thermal Overload RTD32-180 NC (95→96) | Feeds F2 contactor coil |

## Power Distribution Summary
| Source | Destination | Protection |
|---|---|---|
| Wall AC Line | EURO S10H-5H fuse block | 25A (PSU branch), 1A (PLC branch) |
| NDR-480-24 +V | Pushbutton commons (Fwd, Rev, DM1, DM2) | 1.5A fast blow via EURO S4LH |
| NDR-480-24 –V | Contactor A2, D2-08TD2 COM, D2-08ND3 COM, D2-04RTD COM | Direct return |
| Wall AC (via power switch) | PLC L terminal | 1A fast blow |
| Wall AC (via power switch) | PSU L terminal | 25A slow blow |
