# NeoDrone v1 wiring diagram

Current planned wiring:

- 4 motors connected directly to board outputs M1-M4
- battery connected to VBAT and GND
- CRSF receiver connected to power and UART (TX/RX + GND)

```mermaid
flowchart LR
  Battery["Battery"] --> FC["NeoDrone v1 Board"]
  FC --> M1["Motor 1"]
  FC --> M2["Motor 2"]
  FC --> M3["Motor 3"]
  FC --> M4["Motor 4"]
  CRSF["CRSF Receiver"] --> FC
```
