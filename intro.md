## Intro

**Symbols**

- **Router**: Circle with arrows pointing in/out
- **Switch**: Box with arrows pointing out

**Switches**

- Allow connectivity between devices in a LAN
- Require router to talk to internet

**Routers**

- Connectivity between LANs

**Firewall**

- Can be place before or after router
- Monitor and control traffic based on rules
- neg-gen firewalls have more advanced filtering

## Interfaces

**Ethernet**

- Collection of protocols and standards
- Speed is bits per second (only 1 bit can arrive at a time)
  - HDD speed could be Bytes per second

**UTP Cable (Copper)**

| Speed    | Name                | IEEE Standard | name       | Max Length |
| -------- | ------------------- | ------------- | ---------- | ---------- |
| 10 Mbps  | Ethernet            | 802.3i        | 10BASE-T   | 100m       |
| 100 Mbps | Fast Ethernet       | 802.3u        | 100BASE-T  | 100m       |
| 1 Gbps   | Gigabit Ethernet    | 802.3ab       | 100-BASE-T | 100m       |
| 10 Gbps  | 10 Gigabit Ethernet | 802.3an       | 10GBASE-T  | 100m       |

- Cables are Unshielded Twisted Pairs
  - 8 wires (4 pairs). Only 4 used for 10&&100 Mbps (1&2, 3&6)

**For 10 or 100Mpbs**

| Device   | TX      | RX      |
| -------- | ------- | ------- |
| Router   | 1 and 2 | 3 and 6 |
| Firewall | 1 and 2 | 3 and 6 |
| PC       | 1 and 2 | 3 and 6 |
| Switch   | 3 and 6 | 1 and 2 |

- Full Duplex: Can transmit and receive at same time
- If connecting PC to PC, or Router to Router you need a cross-over cable (so you dont connect TX to TX)
  - Most devices now have **Auto MDI-X** to detect and fix incorrect cables

**Gigabit Eth**

- Wires are bi-directional

**Fibre Cable**

- Made up of
  - Fiberglass core
  - cladding to reflect light
  - protective buffer
  - outter jacket
- Types:
  - Single-Mode
    - Lazer transmitter
    - Long cables (up to 30km)
    - expensive
  - multi-mode
    - Core is wider
    - allows multiple modes/angles
    - shorter cables than single-mode (550m @ 1Gpbs, 400@10)
    - cheaper (LED transmitter)

| Speed  | Name        | IEEE Standard | Type  | Length             |
| ------ | ----------- | ------------- | ----- | ------------------ |
| 1Gpbs  | 1000BASE-LX | 802.3z        | SM/MM | 550m (MM) 5km (SM) |
| 10Gpbs | 10GBASE-SR  | 802.3ae       | MM    | 400m               |
| 10Gpbs | 10GBASE-LR  | 802.3ae       | SM    | 10km               |
| 10Gpbs | 10GBASE-ER  | 802.3ae       | SM    | 30km               |
