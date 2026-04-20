# Requirements

## Must (M)
| ID | Requirement |
|---|---|
| M1 | Electrical system must safely support shredding plastic into ~1" pieces when integrated with ME system |
| M2 | Controllable VFD must be used |
| M3 | Electrical design must follow NFPA-70 (NEC) guidance |
| M4 | Emergency stop must safely shut down the system |
| M5 | Overcurrent and overload protection must be included |
| M6 | At least one safety interlock must be used |
| M7 | Motor speed must operate around 70–90 RPM |
| M8 | VFD must support a 3–5 HP motor |
| M9 | System must include an HMI for operator control and status display |
| M10 | Total project cost (EE + ME) must remain under $3,000 |

## Should (S)
| ID | Requirement |
|---|---|
| S1 | System should include clear status and fault indicators |
| S2 | Electrical enclosure should follow NEMA-guided practices |
| S3 | Controls should be clearly labeled and easy to understand |

## May (O)
| ID | Requirement |
|---|---|
| O1 | EE electrical cost may target ~$1,000 (subject to change) |
| O2 | Wireless monitoring may be explored (read-only) |
| O3 | Data logging may be implemented |
| O4 | Additional safety sensing (capacitive touch, thermal) may be explored |

## Performance Specs
| Parameter | Value |
|---|---|
| Target shred size | ~1 inch |
| Motor shaft speed | 70–90 RPM (adjustable via VFD) |
| Plastic materials | High-density PVC, PP, LDPE |
| Plastic thickness | 0.25–0.5 inch |
| Plastic width | 4–12 inch |
| Power input | 120 VAC or 208–240 VAC facility supply |
| Total budget | $3,000 (EE + ME) |

## Pass/Fail Test Criteria
- Shreds plastic into ~1" pieces
- VFD controls motor speed with safe start/stop
- E-stop immediately shuts down the system
- Safety interlocks prevent operation when access points are open
- Overcurrent/overload protection triggers under unsafe electrical conditions
- System operates at ~80–90 RPM without electrical faults or exposed wiring
