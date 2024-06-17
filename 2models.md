## OSI Model

### 7 - Application

- HTTP/HTTPS
- Process to process

### 6 - Presentation

- Translate application data in to network
- eg encryption/decryption

### 5 - Session

### 4 - Transport

- Adds header -> This is segment
- Segment data to send over the network
- Host to Host communication

### 3 - Network

- Adds header -> This is a packet
- Logical addressing [IP]
- path selection between src/dst
- Routers operate here

### 2 - Data Link

- Adds header & trailer -> This is a frame
- Node to Node connectivity
  - PC to switch; switch to router
- Error correcting in physical layer
- Addressing
- Switches operate here

### 1 - Physical

- Voltage; distances; cables
- Converting bits to electrical/radio signals
- No header, but -> This is Bits

## TCP/IP

| OSI          | TCP         |
| ------------ | ----------- |
| Application  | Application |
| Presentation | Application |
| Session      | Application |
| Transport    | Transport   |
| Network      | Internet    |
| Data Link    | Link        |
| Physical     | Link        |
