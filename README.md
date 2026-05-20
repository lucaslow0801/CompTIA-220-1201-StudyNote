# CompTIA A+ Core 1 (220-1201) Study Notes

---

## Table of Contents

1. [1.0 Mobile Devices](#10-mobile-devices)
2. [2.0 Networking](#20-networking)
3. [3.0 Hardware](#30-hardware)
4. [4.0 Virtualization and Cloud Computing](#40-virtualization-and-cloud-computing)
5. [5.0 Hardware and Network Troubleshooting](#50-hardware-and-network-troubleshooting)

---

# 1.0 Mobile Devices

## 1.1 Laptop Hardware

### Battery
- Power source when unplugged; may be easily replaced or require a teardown
- **Lithium-Ion (Li-ion) and Lithium-Ion Polymer (LiPo)** are most common — no "memory effect," charging does not diminish capacity
- Different form factor for each laptop; battery technology is constantly changing

### Keyboard
- Most-used laptop component; can be easy to replace (a few screws and a single ribbon cable — or not)
- Alternative: connect an external USB keyboard
- Some repairs require careful removal/replacement of individual key caps

### Memory (RAM)
- Uses **SO-DIMM** (Small Outline Dual In-line Memory Module)
- Often easy to install and replace
- Some laptop memory is soldered to the system board → no upgrade possible; requires full board replacement

### Storage
| Type | Details |
|------|---------|
| Magnetic HDD | Spinning platters; 2.5" form factor (vs. 3.5" for desktops) |
| SSD (2.5") | All memory, no moving parts; silent, fast, low latency |
| M.2 | Smaller form factor; no SATA data/power cables; easy to install |

### Wireless & Bluetooth
- **802.11 Wi-Fi** — LAN, high speed, internet access
- **Bluetooth** — PAN, short range, connects peripherals and nearby devices
- Often integrated into the motherboard

### Biometrics
- Fingerprint reader or face recognition — "something you are"
- Requires additional OS configuration and hardware
- Relatively secure (faces and fingerprints are quite unique)

### Near-Field Communication (NFC)
- Common on mobile phones and smartwatches
- Short-distance networking: **≤4 centimeters**
- Uses: payment, authentication, data transfers
- Examples: hospital workstations, warehouses, manufacturing

### Wi-Fi Antennas
- Multiple antennas: Wi-Fi main/aux + Bluetooth
- Antenna wires wrap around the laptop screen (foils taped to top or sides of screen)

### Camera & Microphone
- Built-in camera and microphone in the display
- Camera: video capture with specialized drivers/software
- Microphone: useful for video calls; not ideal for non-casual use — analog or USB mics are better

---

## 1.2 Connecting Mobile Devices

### USB Types
| Connector | Description |
|-----------|-------------|
| USB (Standard) | High-speed wired; charging and data transfer |
| Micro-USB | Smaller; common worldwide |
| Mini-USB | Slightly larger; older devices |
| USB-C | 24-pin double-sided; USB 2.0/3.0/3.1/4; also carries DisplayPort, HDMI, Thunderbolt |

### Lightning (Apple)
- Proprietary 8-pin connector for iPhone/iPad
- Higher power output; can be inserted either way; simpler design than Micro-USB

### NFC
- Sends small amounts of data wirelessly over a limited area
- Built into phones; uses: payment, transport, in-person info exchange
- Short range with encryption support; device pairing and data exchange

### Bluetooth
- High-speed PAN communication
- Connects: smartphones, tethering, headsets, health monitors, cars, smartwatches, speakers

### Hotspot / Tethering
- Turns your phone into a personal Wi-Fi router
- Extends cellular data network to all nearby devices
- Dependent on phone type and provider; may require additional charges

### Other Accessories
| Accessory | Description |
|-----------|-------------|
| Stylus | Digital; pressure-sensitive, programmable buttons; must be compatible (e.g., Apple Pencil for iPad) |
| Headsets | Wired (USB, 3.5mm TRRS, Lightning) or Wireless (Bluetooth) |
| Speakers | Battery-powered, Bluetooth wireless |
| Webcam | Internal or external; accessible from multimedia and video conferencing apps |
| Docking Station | Extends laptop interfaces; adds external KB/mouse, additional ports, desktop adapter cards |
| Port Replicator | Similar to docking station but no expansion card; usually connects via USB |
| Trackpad | Replaces mouse; supports multi-finger gestures (right-click, zoom, window control) |
| Drawing Pad | External digitizer with active stylus; very precise input |
| TrackPoint | Small pointing stick embedded in a keyboard for precise cursor control |

---

## 1.3 Mobile Device Networks

### Cellular Generations
| Generation | Details |
|-----------|---------|
| **3G** | Introduced 1998; several Mbps; enabled GPS, mobile TV, video conferencing |
| **4G / LTE** | Based on GSM/EDGE; 150 Mbit/s download |
| **LTE-A** | 300 Mbit/s download |
| **5G** | Launched 2020; up to 10 Gbps; major IoT impact; 100–900 Mbit/s at slower speeds |

- Airplane mode disables all cellular networks; can also disable data while keeping voice

### Wi-Fi
- Connects to local 802.11 for data/email/internet; requires a local access point
- Supports Wi-Fi calling (requires carrier support)

### Hotspot
- Phone becomes a personal wireless router
- Extends cellular data to all devices; may require extra charges

### SIM (Subscriber Identity Module)
- Tiny physical card containing carrier info, SIM ID, phone number, storage for contacts/messages
- **eSIM** — embedded SIM; cannot be physically removed
- Many devices support multiple SIMs

### Bluetooth Pairing Steps
1. Enable Bluetooth on both devices
2. Set both devices to discoverable mode
3. Select the discovered device
4. Enter or confirm PIN (must match on both)
5. Test connectivity — future connections should be automatic

### GPS
- Created by U.S. Department of Defense; 30+ satellites in orbit
- Needs at least **4 satellites** for precise navigation
- Determines: longitude, latitude, altitude
- Mobile uses: maps, directions, location services, geotracking

---

## 1.3 Mobile Device Management (MDM)

### MDM Overview
- Manages company-owned and user-owned (BYOD) mobile devices
- Centralized control: apps, data, camera, access control, PINs, screenshots

### Device Ownership Models
| Model | Description |
|-------|-------------|
| **BYOD** (Bring Your Own Device) | Employee owns the device; must meet company requirements; difficult to secure |
| **COPE** (Corporate Owned, Personally Enabled) | Company buys device; used for both work and personal; full corporate control |
| **CYOD** (Choose Your Own Device) | Similar to COPE but user picks the device |

### MDM Policy Enforcement
- **Corporate email** — auto-configured by MDM (no manual setup needed)
- **Two-factor authentication** — biometrics, authentication apps
- **App control** — allow or restrict installations; prevent unauthorized usage

### Data Synchronization
- Syncs: calendar, contacts, email, phone/text settings
- Manages data caps, transfer costs, and cellular vs. Wi-Fi usage
- Can enable/disable network connections remotely

---

# 2.0 Networking

## 2.1 Introduction to IP

### TCP vs. UDP

| Feature | TCP | UDP |
|---------|-----|-----|
| Connection | Connection-oriented (3-way handshake) | Connectionless |
| Reliability | Reliable; error recovery, retransmission | Unreliable; no error recovery |
| Flow Control | Yes — receiver controls data rate | No — sender decides |
| Use Cases | HTTPS, SSH | DHCP, TFTP, real-time comms |

---

## 2.1 Common Ports

| Protocol | Port | Transport | Description |
|----------|------|-----------|-------------|
| FTP | 20 (data), 21 (control) | TCP | File transfer; username/password auth |
| SSH | 22 | TCP | Encrypted remote login |
| Telnet | 23 | TCP | Unencrypted remote login (not recommended for production) |
| SMTP | 25 | TCP | Server-to-server email transfer; sending mail from device |
| DNS | 53 | TCP/UDP | Converts domain names to IP addresses |
| DHCP | 67 (server), 68 (client) | UDP | Automatic IP address assignment |
| HTTP | 80 | TCP | Unencrypted web communication |
| HTTPS | 443 | TCP | Encrypted web communication |
| POP3 | 110 | TCP | Download email from server (emails deleted from server) |
| IMAP | 143 | TCP | Sync email across devices (emails stay on server) |
| SMB | 445 | TCP | Windows file/printer sharing (also called CIFS) |
| LDAP | 389 | TCP | Directory access (e.g., Active Directory) |
| RDP | 3389 | TCP | Remote desktop access |

---

## 2.2 Wireless Network Technology

### IEEE 802.11 Standards (Wi-Fi Generations)
| Standard | Wi-Fi Name |
|----------|-----------|
| 802.11ac | Wi-Fi 5 |
| 802.11ax | Wi-Fi 6 / Wi-Fi 6E |
| 802.11be | Wi-Fi 7 |

- **Frequencies:** 2.4 GHz, 5 GHz, 6 GHz (sometimes combined)
- **Channels:** Grouped frequencies numbered by IEEE; using non-overlapping channels is optimal
- **Bandwidth:** 20 MHz, 40 MHz, 80 MHz, 160 MHz, etc.

### Bluetooth
- Uses the **2.4 GHz** unlicensed ISM band (same as 802.11)
- Short range — most consumer devices: ~10 meters
- Applications: headsets, speakers, keyboards

### RFID (Radio Frequency Identification)
- Used for: access badges, inventory tracking, pet ID, asset tracking
- Radar technology: radio energy powers the tag; tag transmits its ID back
- Some tags can be active/powered; bidirectional communication

### NFC (Near Field Communication)
- Two-way wireless; builds on RFID (mostly one-way)
- Uses: payment systems, Bluetooth pairing, access tokens, identity cards
- Short range with encryption support

---

## 2.3 Network Services

| Service | Description |
|---------|-------------|
| **DNS Server** | Converts names ↔ IP addresses; distributed; managed by ISP or IT |
| **DHCP Server** | Automatic IP configuration; available on most home routers; enterprise servers are redundant |
| **File Share** | Centralized document storage using SMB, AFP, etc. |
| **Print Server** | Provides network printing via SMB, IPP, LPD; can be software or built into printer |
| **Syslog** | Standard message logging; feeds into SIEM; requires lots of disk space |
| **Web Server** | Responds to HTTP/HTTPS requests; serves static or dynamic HTML pages |
| **Database Server** | Stores data in relational tables; uses SQL (MS SQL, MySQL, etc.) |
| **NTP Server** | Provides time synchronization; critical for encryption, logins, backups, logs |
| **Spam Gateway** | Filters unwanted email before it reaches users; on-site or cloud-based |
| **Load Balancer** | Distributes load across multiple servers; provides fault tolerance |
| **Proxy Server** | Intermediate server for access control, caching, URL filtering, content scanning |

### AAA Server (Authentication, Authorization, Accounting)
- Central login management; almost always an enterprise service with redundant servers
- **RADIUS** — UDP-based; combines auth + authorization; used for VPNs and Wi-Fi
- **TACACS+** — TCP-based; separates auth, authorization, and accounting; used for device administration

### SCADA / ICS
- Large-scale, multi-site Industrial Control System
- Manages: power generation, refining, manufacturing, logistics
- Requires extensive network segmentation; no outside access

### Legacy & Embedded Systems
- **Legacy systems** — old but critical; unable to receive security updates; often isolated
- **Embedded systems** — designed for a specific purpose (alarm systems, PLCs, time card systems)

### IoT (Internet of Things)
- Appliances, smart speakers, thermostats, smart doorbells
- May require a **segmented network** to limit security breaches

---

## 2.4 DNS Configuration

| Record Type | Purpose |
|-------------|---------|
| **A** | Maps hostname → IPv4 address |
| **AAAA** | Maps hostname → IPv6 address |
| **CNAME** | Alias for another hostname (e.g., `www.example.com` → `example.com`) |
| **MX** | Specifies the mail server hostname for a domain |
| **TXT** | Human-readable text; used for security/verification |

### TXT Record Security Uses
- **DKIM** — Adds a digital signature to emails; public key stored in TXT record
- **SPF** — Lists authorized mail servers; prevents spoofing
- **DMARC** — Policy for what to do when SPF/DKIM fail (accept / send to spam / reject)

---

## 2.4 DHCP

### DORA Process (How a device gets a lease)
1. **Discovery** — Client broadcasts: "Is there a DHCP server? I need an IP!"
2. **Offer** — Server responds: "Here is 192.168.1.50 for you."
3. **Request** — Client: "I'll take it! Please assign 192.168.1.50 to me."
4. **Acknowledgment (ACK)** — Server: "Done! You have a lease for the next 24 hours."

### DHCP Concepts
| Concept | Description |
|---------|-------------|
| **Reservations** | Assign a fixed IP to a specific MAC address ("Reserved sign") |
| **Scope** | The range of IPs the DHCP server can hand out (e.g., 192.168.1.100–200) |
| **Exclusions** | IPs carved out of the scope that DHCP will never assign (e.g., reserved for printers) |

---

## 2.4 VLANs and VPNs

### VLAN (Virtual Local Area Network)
- Logically segments a physical network into smaller, private groups
- Hosts communicate as if on the same broadcast domain regardless of physical location

### VPN (Virtual Private Network)
- Creates a secure encrypted tunnel over a public network

| VPN Type | Description |
|---------|-------------|
| **Remote Access VPN** (Client-to-Site) | Software on a device connects it to the office network (e.g., Cisco AnyConnect) |
| **Site-to-Site VPN** | Connects two entire buildings via routers; creates a permanent bridge |

---

## 2.5 Networking Hardware Devices

### Router
- Forwards data packets between different networks; connects home network to the internet
- Operates based on **IP addresses**

### Switches
- Core of enterprise networks; forwards traffic based on MAC addresses (using ASICs)
- May provide **PoE** (Power over Ethernet)

| Switch Type | Description |
|-------------|-------------|
| **Unmanaged** | Plug-and-play; no VLAN; no management protocols; low cost |
| **Managed** | VLAN support (802.1Q), traffic prioritization, redundancy, port mirroring, SNMP |

### Access Point (AP)
- Bridges wired network to wireless; not a router
- Makes forwarding decisions based on MAC addresses; extends LAN to Wi-Fi

### Patch Panel
- Combines punch-down blocks and RJ-45 connectors for cable management
- Desk runs are permanently punched down; patch cables connect panel to switch
- Moving a user = just move the patch cable, not rewire the building

### Firewalls
- Filters traffic by port number (OSI Layer 4 — TCP/UDP)
- Can encrypt traffic, proxy traffic, and act as a Layer 3 router
- **Network-based** — protects entire network (physical box or router feature)
- **Host-based** — software on a specific PC (e.g., Windows Defender Firewall)

### Power over Ethernet (PoE)
- Delivers power and data over a single Ethernet cable

| Standard | Power |
|----------|-------|
| PoE | 15.4W DC, 350 mA max |
| PoE+ | 25.5W DC, 600 mA max |
| PoE++ Type 3 | 51W, 600 mA max |
| PoE++ Type 4 | 71.3W, 960 mA max |

- **PoE Injector (Midspan)** — used when switch doesn't support PoE; "injects" power into the cable

### Modem Types
| Type | Description |
|------|-------------|
| **Cable Modem** | Uses DOCSIS over cable TV infrastructure; up to 1 Gbps |
| **DSL Modem** | Uses telephone lines; asymmetric (200 Mbit/s down / 20 Mbit/s up); 10,000 ft CO limit |
| **ONT** (Optical Network Terminal) | Fiber to premises; converts fiber (ISP side) to copper (your network side) |

### NIC (Network Interface Card)
- Every network device has one; often built into the motherboard
- Contains a unique **MAC address** (Media Access Control)

---

## 2.6 IPv4 and IPv6

### IPv4
- 32-bit address; expressed in decimal

| Address Type | Range | Class |
|-------------|-------|-------|
| Private Class A | 10.0.0.0 – 10.255.255.255 | Large corporations |
| Private Class B | 172.16.0.0 – 172.31.255.255 | — |
| Private Class C | 192.168.0.0 – 192.168.255.255 | Home routers |

- **Public IPs** — assigned by ISPs; globally unique; internet-routable

### IPv6
- 128-bit address; expressed in hexadecimal
- No more private/public split — every device can have a unique global address
- **Link-Local Address** — auto-assigned `fe80::` prefix; local communication without a router

### APIPA (Automatic Private IP Addressing)
- Self-configured when DHCP server is unavailable
- Range: **169.254.0.0 – 169.254.255.255**
- Valid only within the local network segment; cannot connect to the internet

### IP Address Types Summary
| Type | Description |
|------|-------------|
| **Static** | Permanent; manually assigned; ideal for servers and network devices |
| **Dynamic** | Assigned by DHCP; changes periodically; used for consumer devices |
| **Subnet Mask** | Identifies network vs. host portion (e.g., `255.255.255.0`) |
| **Default Gateway** | Router that enables communication between different subnets |

---

## 2.7 Network Connection Types

| Type | Details |
|------|---------|
| **Satellite** | Non-terrestrial; 100 Mbit/s down / 5 Mbit/s up; high latency (250 ms); Starlink: 25–60 ms |
| **Fiber** | Light-based; high cost; long distance; SONET/WDM; very high data rates |
| **Cable** | DOCSIS over cable TV; 50–1000+ Mbit/s; supports data, voice, video |
| **DSL (ADSL)** | Telephone lines; 200/20 Mbit/s; 10,000 ft CO limit |
| **Cellular** | Cell-based coverage; supports tethering and mobile hotspot |
| **WISP** | Wireless ISP for rural areas; meshed 802.11, 5G home internet, or proprietary wireless |

---

## 2.7 Network Types

| Type | Scope | Technology |
|------|-------|-----------|
| **LAN** | Building or group of buildings | Ethernet, 802.11 |
| **WAN** | Global; connects LANs | MPLS, point-to-point serial |
| **PAN** | ~10 meters | Bluetooth, USB |
| **MAN** | City / campus (5–50 km) | Metro Ethernet, Fiber, Microwave |
| **SAN** | Storage network | Fibre Channel, iSCSI |
| **WLAN** | Wireless LAN | IEEE 802.11 (Wi-Fi) |

---

## 2.8 Network Tools

| Tool | Purpose |
|------|---------|
| **Cable Crimper** | Attaches RJ-45 connectors to Ethernet cables |
| **Cable Stripper** | Removes insulation from wire ends |
| **Wi-Fi Analyzer** | Measures signal strength, detects interference, analyzes channel usage |
| **Toner Probe** | Traces and identifies individual wires in a cable bundle |
| **Punch Down Tool** | Attaches network cables to a patch panel |
| **Cable Tester** | Verifies cable integrity and connectivity; identifies missing pins or crossed wires |
| **Loopback Plug** | Tests NIC and physical port functionality |
| **Network Tap** | Monitors network traffic without interrupting data flow |

---

# 3.0 Hardware

## 3.1 Display Types

### LCD (Liquid Crystal Display)
| Panel Type | Color Quality | Viewing Angles | Response Time |
|-----------|--------------|----------------|---------------|
| **TN** (Twisted Nematic) | Low | Narrow | Fast |
| **IPS** (In-Plane Switching) | High | Wide | Fast |
| **VA** (Vertical Alignment) | Good | Good | Slow |

### OLED (Organic Light-Emitting Diode)
- No backlight — the organic compound itself emits light
- Exceptional contrast and black levels; thinner and lighter
- Risk of **burn-in** from static images over thousands of hours

### Mini-LED
- Same backlight tech as LED-backlit LCD but with much smaller LEDs
- Better control over dark areas; deeper blacks; excellent contrast; high peak brightness

### Touch Screen / Digitizer
- Performs both input and output; translates analog touch into digital data
- Supports stylus input; used in laptops, tablets, and hybrid devices

### Inverter (Legacy CCFL Displays)
- Converts low-voltage DC (from motherboard) to high-voltage AC (for CCFL backlight)
- **LED displays do not use an inverter** — they run on low-voltage DC directly

---

## 3.1 Display Attributes

| Attribute | Description |
|-----------|-------------|
| **Pixel Density** | Pixels per inch (PPI); higher = sharper image |
| **Refresh Rate** | Times per second the screen updates (Hz); movies: 24fps, games: 60fps+ |
| **Screen Resolution** | Total pixels: 720p (1280×720), 1080p (1920×1080), 1440p (2560×1440), 4K (3840×2160) |
| **Color Gamut** | Range of colors the display can reproduce; OLEDs typically have a wide gamut |

---

## 3.2 Network Cables

### Copper
| Type | Description |
|------|-------------|
| **T568A / T568B** | Twisted-pair pinout standards for RJ-45 connectors |
| **Coaxial** | Single copper conductor with insulation and shielding; used for cable TV and broadband |
| **STP** (Shielded Twisted Pair) | Extra shielding reduces external interference |
| **Direct Burial STP** | Enhanced shielding; water/chemical resistant; for underground use |
| **UTP** (Unshielded Twisted Pair) | Most common; no extra shielding |

- **Plenum-rated** — fire-retardant jacket; required in building air-handling spaces (between dropped ceiling and structural ceiling)

### Fiber Optic
| Type | Distance | Cost | Light Source |
|------|----------|------|-------------|
| **Single-mode** | >100 km | Higher | Laser |
| **Multimode** | Up to 2 km | Lower | LED |

### USB Cables
| Version | Speed |
|---------|-------|
| USB 2.0 | 480 Mbps; max 5m |
| USB 3.0 | 5 Gbps (SuperSpeed) |
| USB 3.1 | 10 Gbps |
| USB 3.2 | 20 Gbps |

### Thunderbolt
| Version | Speed |
|---------|-------|
| Thunderbolt 1 | 20 Gbps (2×10 Gbps) |
| Thunderbolt 2 | 20 Gbps (unified) |
| Thunderbolt 3 | 40 Gbps |

- Copper: up to 3 meters; Fiber-optic: up to 60 meters; Daisy-chain up to 6 devices

### Video Cables
| Cable | Audio | Signal |
|-------|-------|--------|
| HDMI | Yes | Digital |
| DisplayPort (DP) | Yes | Digital |
| DVI-A | No | Analog |
| DVI-D | No | Digital |
| DVI-I | No | Digital + Analog |
| VGA | No | Analog |
| USB-C | Via adapter | Digital (DisplayPort / HDMI) |

### SATA
- **Power connector:** 15 pins; **Data connector:** 7 pins; one device per cable

| Version | Speed |
|---------|-------|
| SATA I | 1.5 Gbps |
| SATA II | 3 Gbps |
| SATA III | 6 Gbps |
| eSATA | 6 Gbps (external) |

---

## 3.3 RAM (Random Access Memory)

### Form Factors
| Type | Use | Pins |
|------|-----|------|
| **DIMM** | Desktops | Separate contacts on each side |
| **SO-DIMM** | Laptops | DDR3: 204 pins; DDR4: 260 pins |

### RAM Types
| Type | Speed | Cost | Use |
|------|-------|------|-----|
| **SRAM** | Faster | More expensive | CPU cache |
| **DRAM** | Slower | Less expensive | Main RAM modules |
| **SDRAM** | Syncs to system clock | — | General use |

### DDR Generations
| Version | Max per Module | Pins |
|---------|---------------|------|
| DDR3 | 16 GB | 240 |
| DDR4 | 32 GB | 288 |
| DDR5 | 64 GB | 288 |

> Note: DDR versions are **not backward compatible**; notch prevents wrong installation.

### Error Correction
- **Parity bit** — extra bit detects (but doesn't correct) data errors
- **ECC (Error-Correcting Code)** — detects and corrects errors; more expensive and slightly slower; used in servers

### Multi-Channel Memory
- Requires matching type, capacity, and speed in color-coded slots on the motherboard

---

## 3.4 Storage Devices

### HDD (Hard Disk Drive)
- Non-volatile magnetic storage; platters spin at RPM (up to 15,000 RPM)
- Form factors: 2.5" and 3.5"

### SSD (Solid State Drive) — Interface Types
| Interface | Speed | Notes |
|-----------|-------|-------|
| **SATA** | Max 6 Gbps | Common in 2.5" SSDs; consumer grade |
| **NVMe** (PCIe) | Up to 20 Gbps | Developed specifically for SSDs; low latency |
| **SAS** | High | Mission-critical; servers and data centers |

### SSD Form Factors
| Form Factor | Notes |
|-------------|-------|
| **M.2 (B-key)** | 2 PCIe lanes (slower) |
| **M.2 (M-key)** | 4 PCIe lanes (faster) |
| **M.2 (B+M key)** | Compatible with both slots; limited to SATA or PCIe x2 speed |
| **mSATA** | Older portable SSD format; superseded by M.2 |

### Removable Storage
- **Flash drives** — plug-and-play USB; general file transfer; non-volatile, rewritable
- **Memory cards** — expand storage in compact electronics; non-volatile, rewritable

### Optical Drive
- CD-ROM, DVD-ROM, Blu-ray; reads microscopic bumps with a laser beam

---

## 3.4 RAID (Redundant Array of Independent Disks)

| RAID Level | Min Drives | Also Known As | Fault Tolerance | Notes |
|-----------|-----------|---------------|----------------|-------|
| **RAID 0** | 2 | Disk Striping | None (any disk failure = full data loss) | Best performance; no redundancy |
| **RAID 1** | 2 | Disk Mirroring | 1 drive failure | Data duplicated on each drive |
| **RAID 5** | 3 | Striping with Parity | 1 drive failure | Performance + fault tolerance |
| **RAID 6** | 4 | Striping with Double Parity | 2 drive failures | Higher redundancy than RAID 5 |
| **RAID 10** | 4 | Stripe of Mirrors | 1 drive per mirrored pair | Combines RAID 0 + RAID 1 |

---

## 3.5 Motherboard

### Form Factors
| Form Factor | Size | Expansion Slots | RAM Slots |
|------------|------|-----------------|-----------|
| **ATX** | Standard desktop | Up to 7 PCIe | 4 DIMM |
| **mATX** | Compact/budget | Up to 4 | Compatible with ATX/mATX cases |
| **ITX** | Smallest | 1 PCIe | Highly compact cases |

### Connector Types
| Connector | Description |
|-----------|-------------|
| **PCI** | Legacy; 32/64-bit bus for sound cards, GPUs, network adapters |
| **PCIe** | Modern standard; x1, x4, x8, x16 lanes; Gen 4/5/6 |
| **24-pin ATX** | Main motherboard power |
| **8-pin EPS** | CPU power (12V) |
| **6/8-pin PCIe** | GPU power |
| **SATA** | L-shaped; storage device power |
| **eSATA** | External storage at internal SATA speeds |
| **Headers** | Front panel pins: power button, reset, USB, LEDs, fans |
| **M.2** | M-key (NVMe x4), B-key (SATA/PCIe x2), B+M key (hybrid) |

### CPU Socket Types
| Manufacturer | Virtualization |
|-------------|---------------|
| **AMD** | AMD-V; generally superior for gaming and efficiency |
| **Intel** | VT-x; often excels in raw speed for productivity |

### Server Motherboard Features
- Multi-socket (multiple physical CPUs)
- 4+ RAM slots; supports ECC RAM
- Many expansion slots; rack-mount / blade form factor

### BIOS / UEFI
| Feature | Description |
|---------|-------------|
| **BIOS** | Legacy firmware; POST → Boot loader → OS |
| **UEFI** | Modern replacement; secure, faster, more features |
| **Boot Menu Keys** | F12, F11, Esc, or Del (varies by manufacturer) |
| **Secure Boot** | Ensures only signed OS/bootloaders run at startup |
| **BIOS Password** | Locks firmware to prevent unauthorized access |
| **USB Permissions** | Enable/disable USB ports and boot from USB |
| **Fan Control** | Adjust RPM relative to temperature |
| **Temperature Monitoring** | Tracks thermal conditions via sensors |
| **Virtualization Support** | Intel VT-x / AMD-V — enables running VMs |

---

## 3.5 TPM and HSM

| Feature | TPM | HSM |
|---------|-----|-----|
| Scope | Single system | Multiple systems |
| Purpose | Secure local device hardware/firmware | Secure cryptographic keys across devices |
| Deployment | Built into motherboard or add-on module | High-end server or data center appliance |
| Security Level | Lower | Higher |

---

## 3.5 CPU Architecture

| Architecture | Description |
|-------------|-------------|
| **x86** | Traditional 32-bit; 32-bit OS cannot run 64-bit apps |
| **x64** | 64-bit extension; also known as AMD64 or Intel 64 |
| **ARM** | Power-efficient RISC-based design; used in mobile devices |

### Core Configurations
| Cores | Use Case |
|-------|---------|
| 2–4 | Basic office work, web browsing |
| 6–8 | Gaming, content creation, modern desktop |
| 10+ | High-end workstations, video editing |

---

## 3.5 Cooling

| Component | Type | Function |
|-----------|------|---------|
| **Fan** | Active | Pulls cool air through the PC |
| **Heat Sink** | Passive | Transfers heat to air or liquid |
| **Thermal Paste / Pad** | Passive | Fills gap between CPU and heat sink for efficient heat transfer |
| **Liquid Cooling** | Active | Uses liquid medium to transfer heat away from components |

---

## 3.6 Power Supply (PSU)

> **Key Formula:** Watt = Volt × Amp (e.g., 60W = 120V × 0.5A)

- Converts wall outlet **AC** (110–240V) → stable **DC** (3.3V, 5V, 12V) for PC components

### AC vs. DC
- **AC (Alternating Current)** — direction constantly reverses; used in wall outlets
- **DC (Direct Current)** — flows in one direction at constant voltage; used by PC components

### Voltage Standards
| Region | Standard |
|--------|---------|
| USA | 110–120 VAC, 60 Hz |
| Europe | 220–240 VAC, 50 Hz |

### Output Rails
| Rail | Used For |
|------|---------|
| +3.3V | NVMe M.2, RAM, motherboard logic |
| +5V | USB ports and devices |
| +12V | Fans, motors, GPU, PCIe cards |

### 20+4 Pin Connector
- Maintains compatibility with both 20-pin and 24-pin motherboards
- Leave the 4-pin section detached for 20-pin boards

### Energy Efficiency (80 PLUS Ratings)
Ratings from least to most efficient: **White → Bronze → Silver → Gold → Platinum → Titanium**

- Typically ranges from 80% to 96% efficiency
- More efficiency = more DC power delivered + less heat generated

### Redundant PSU (Servers)
- Two or more PSUs; each can handle 100% of the load (normally runs at 50%)
- **Hot-swappable** — replace a faulty PSU without powering down

---

## 3.7 Multifunction Devices / Printers (MFD / MFP)

### Printer Languages
| Language | Best For |
|----------|---------|
| **PCL** | High-volume, everyday printing; less resource-intensive |
| **PostScript** | Professional design, desktop publishing; slower but higher quality |

> Always match the driver to the printer language (PCL → PCL driver; PostScript → PostScript driver)

### Device Connectivity
| Method | Notes |
|--------|-------|
| USB | Direct wired connection to a single computer |
| Ethernet | RJ-45; network printing |
| Bluetooth | Limited range |
| Wi-Fi (Infrastructure) | Multiple devices via access point |
| Wi-Fi (Ad hoc) | Direct link between wireless devices |

### Print Server vs. Printer Share
| Method | Advantage | Disadvantage |
|--------|-----------|-------------|
| **Printer Share** | Easy setup | Requires host PC to be on; limited control; can bottleneck |
| **Print Server** | Highest availability; web-based management; jobs queued on printer | More setup required |

### Configuration Settings
| Setting | Description |
|---------|-------------|
| Duplex | Print on both sides of paper |
| Orientation | Portrait (default) or Landscape |
| Tray Settings | Select paper size/type per tray |
| Quality | Draft → Normal → Best → Maximum DPI |

### Security
- **User authentication** — set rights/permissions for printing vs. managing
- **Badging** — employee badge required to release print jobs
- **Audit logs** — tracks all printer activities
- **Secured prints (PIN printing)** — job held until PIN entered at printer

### Scan Services
| Method | Description |
|--------|-------------|
| Email (SMTP) | Scanned document sent to inbox |
| SMB | Scanned document saved to a network shared folder |
| Cloud | Scan to Google Drive, Dropbox, etc. |

### Scanner Types
- **ADF (Automatic Document Feeder)** — processes multi-page documents automatically
- **Flatbed Scanner** — document placed face down on glass; scanning mechanism moves underneath

---

## 3.8 Printer Maintenance

### Laser Printer
- **Maintenance kit** — prepackaged replacement parts for components with limited lifespan
- **New toner cartridge** — gently rock horizontally several times before installing to distribute toner evenly
- **Cleaning tools** — toner vacuum, toner cleaning wipes, isopropyl alcohol

### Inkjet Printer
- **Ink cartridge** — replaceable; applies color to the page
- **Printhead** — sprays microscopic ink droplets; clean with built-in cycle or lint-free cloth + isopropyl alcohol / distilled water
- **Roller** — moves paper through the printer
- **Feeder** — picks up paper from the input tray
- **Calibration** — corrects color and alignment issues
- **Paper jams** — caused by incorrect paper type, dirty rollers, overloaded tray

### Thermal Printer
- **Feed assembly** — moves paper through the printer; maintain by cleaning rollers with isopropyl alcohol
- **Storage** — keep thermal paper cool and dry, away from sunlight and heat
- **Heating element** — clean periodically with lint-free cloth or cleaning card + isopropyl alcohol
- **Maintenance** — remove dust from rollers with compressed air or soft brush

### Impact Printer (Dot Matrix)
- Uses **multipart paper** to create duplicate copies
- Paper handling: align perforated edges in the tractor feed mechanism

---

# 4.0 Virtualization and Cloud Computing

## 4.1 Virtualization

### Purpose of Virtual Machines
- **Sandbox Testing** — safe, isolated environment to test risky software without harming the host
- **Test / Development** — create, deploy, and test software in various OS environments; use snapshots to revert state
- **Application Virtualization** — run legacy software, different app versions, or cross-platform software

### Requirements
- **CPU** — multi-core with Intel VT-x or AMD-V enabled in BIOS/UEFI
- **RAM** — high capacity (8 GB minimum recommended for multiple VMs)
- **Storage** — fast SSD for virtual disk files

### Hypervisor Types
| Type | Description | Examples |
|------|-------------|---------|
| **Type 1 (Bare Metal)** | Hypervisor IS the OS; runs directly on hardware | VMware ESXi, Hyper-V |
| **Type 2 (Hosted)** | Hypervisor runs within an existing OS | VirtualBox, VMware Workstation |

### Hypervisor Networking
| Mode | Description |
|------|-------------|
| **Shared (NAT)** | VM gets IP from virtual DHCP; uses host IP for outbound; not visible on LAN |
| **Bridged** | VM connects directly to physical network; behaves like any physical machine |

### Hypervisor Security
- **VM escaping** — malware recognizes it's in a VM, compromises the hypervisor, and jumps to other VMs
- Hosted services are often virtual; malware on one customer's server can potentially reach others

### Containers
- Lightweight OS-level technology packaging applications and dependencies
- Run in isolated environments on a shared host OS kernel (no full OS per container)

### Desktop Virtualization
- **DVI (Desktop Virtualization Infrastructure)** — applications run on a remote server; local device = keyboard, mouse, screen
- **DaaS (Desktop as a Service)** — cloud-based desktop virtualization

---

## 4.2 Cloud Computing

### Cloud Deployment Models
| Model | Description |
|-------|-------------|
| **Private** | Exclusively used by one organization; strict compliance/security |
| **Public** | Available to everyone; shared across multiple organizations |
| **Hybrid** | Mix of public and private clouds |
| **Community** | Shared by several organizations with similar needs (e.g., universities, government agencies) |

### Cloud Service Models
| Model | Description |
|-------|-------------|
| **IaaS** (Infrastructure as a Service) | Rent computing infrastructure; hardware managed by provider |
| **PaaS** (Platform as a Service) | Cloud platform for developers to build and deploy apps |
| **SaaS** (Software as a Service) | Access software via browser; subscription-based (e.g., email, Office 365) |

### Cloud Characteristics
| Characteristic | Description |
|----------------|-------------|
| **Shared Resources** | Multiple customers share physical infrastructure; lower cost but variable performance |
| **Dedicated Resources** | Reserved for one customer; consistent performance; higher cost (= private cloud) |
| **Metered Utilization** | Pay based on actual usage; ingress (data in) and egress (data out) costs |
| **Elasticity** | Resources scale up/down automatically based on demand |
| **Availability** | Systems always accessible; redundancy ensures minimal interruption; SLA defines uptime (e.g., 99.9%) |
| **File Synchronization** | File edits on one device reflect across all connected devices |
| **Multitenancy** | Multiple customers share one deployment without accessing each other's data |

---

# 5.0 Hardware and Network Troubleshooting

## 6-Step Troubleshooting Methodology

1. **Identify the problem**
2. **Establish a theory of probable cause** (question the obvious)
3. **Test the theory to determine the cause**
4. **Establish a plan of action and implement the solution**
5. **Verify full system functionality** and implement preventative measures
6. **Document the findings, actions, and outcomes**

---

## 5.1 Hardware Troubleshooting

### POST (Power-On Self-Test) Beep Codes
| Beep Pattern | Meaning |
|-------------|---------|
| No beep | No power, dead motherboard, or failed CPU |
| 1 beep | System OK (BIOS dependent) |
| Repeating beeps | RAM, GPU, or CPU issue |

> **Fix:** Check BIOS beep codes, reseat RAM/GPU, clear CMOS, test parts individually

### Common Hardware Issues

| Symptom | Common Causes | Fixes |
|---------|--------------|-------|
| **BSOD / Mac Pinwheel** | Bad RAM, overheating, driver/hardware conflict | Run memory diagnostics, check Event Viewer, update BIOS/drivers |
| **Blank Screen** | GPU/RAM not seated, CPU/motherboard fault | Test monitor, reseat components, test one RAM stick |
| **No Power** | Bad PSU, loose cable, damaged power button, wrong voltage | Test PSU, check connections, verify voltage — never open a PSU |
| **Sluggish Performance** | Failing RAM, overheating, dust, malware | Task Manager, clean dust, reapply thermal paste, malware scan |
| **Overheating** | Bad cooling, dried thermal paste, poor airflow, overclocking | Clean fans, reapply paste, add case fans, monitor temps |
| **Burning Smell** | Failing PSU, fried capacitor, overheated CPU | Power off immediately, inspect/replace components |
| **Random Shutdowns** | Overheating, power surges, RAM/PSU failure | Monitor temps, use surge protector, test RAM, update BIOS |
| **Application Crashes** | Faulty RAM/CPU, software conflict, malware | Run `sfc /scannow`, test RAM, check Reliability Monitor |
| **Unusual Noises** | Fan bearings, loose cables, coil whine | Clean/secure cables, replace fans |
| **Capacitor Swelling** | Degraded components → instability, freezes | Replace the motherboard |
| **Wrong Date/Time** | Dead CMOS battery (CR2032) | Replace battery, reset BIOS date/time |

---

## 5.2 Troubleshoot Drives and RAID

### RAID LED Status
| Color | Meaning |
|-------|---------|
| Green | Drive operating normally |
| Amber / Yellow | Warning or minor issue |
| Red | Critical failure |

### Common Drive Issues

| Symptom | Cause | Action |
|---------|-------|--------|
| **Grinding noise** | Worn/misaligned heads or spindle | Stop immediately; backup data |
| **Clicking sounds** | Actuator arm can't find data sectors | Near-total failure; backup and replace |
| **Bootable device not found** | Corrupted OS, failed RAID member, BIOS misconfiguration | Verify BIOS and RAID integrity |
| **Data loss / corruption** | Power loss, RAID sync failure, physical issues | Use recovery tools; attempt RAID rebuild |
| **S.M.A.R.T. failure** | High temps, read/write errors, bad sectors | Backup immediately; replace drive |
| **Extended read/write times** | Bad sectors, degraded RAID, overworked controller | Use S.M.A.R.T. tools; replace slow drives |
| **Low IOPS** | Degraded disks, fragmentation, network bottlenecks | Check RAID health, defragment, upgrade drives |
| **Missing drives in OS** | Loose cables, bad sectors, misconfigured arrays | Verify connections, check RAID setup |
| **Array missing** | Drive failures, controller issues, improper shutdown | Re-seat drives, check cables; do NOT reinitialize |
| **Audible alarms** | Hardware fault alert | Check manufacturer manual for alarm meaning |

---

## 5.3 Display Troubleshooting

| Symptom | Cause | Fix |
|---------|-------|-----|
| **No signal / blank screen** | Incorrect input source | Verify input (HDMI/VGA/DP); use Win+P to toggle |
| **Flickering / distorted image** | Loose or damaged cables | Reseat or replace cables |
| **Dim projector** | Burnt-out bulb | Replace lamp; check cooling |
| **Fuzzy / blurry image** | Wrong resolution | Set native resolution; use quality cables |
| **Burn-in** | Static image left on OLED screen | Enable screen saver; lower brightness |
| **Dead pixels** | Stuck pixels | Try pixel-repair software; warranty replacement |
| **Flickering screen** | Bad cable or graphics driver | Check cables; update drivers; adjust refresh rate |
| **Incorrect colors** | Display calibration off | Calibrate via OSD or graphics settings |
| **Dim laptop screen** | Failed inverter (CCFL) or backlight issue | Adjust brightness; replace inverter |
| **Projector shuts off** | Overheating | Clean vents; check fans; check cooling system |
| **Distorted/stretched image** | Wrong resolution or aspect ratio | Adjust aspect ratio and resolution; reseat video cable |

---

## 5.4 Mobile Device Troubleshooting

| Symptom | Cause | Fix |
|---------|-------|-----|
| **Poor battery health** | Battery wear from charge cycles, heat, heavy usage | Check battery health; reduce background apps; replace battery if needed |
| **Swollen battery** | Lithium-ion breakdown; gas buildup | Stop use immediately; take to certified repair center; dispose at e-waste |
| **Broken screen** | Physical damage | Assess damage; apply temp protector; replace screen |
| **Improper charging** | Faulty port, cable, or power source | Test different charger; clean port; replace port if damaged |
| **Poor / no connectivity** | Wi-Fi, Bluetooth, or cellular issue | Toggle Airplane mode; restart; forget and reconnect; reset network settings |
| **Liquid damage** | Short circuits from moisture | Power off; remove SIM/cards; dry with silica gel (48h); take to repair center |
| **Overheating** | Resource-heavy apps, direct sunlight, malware | Close background apps; remove case; restart; run malware scan |
| **Digitizer issues** | Touch not registering or ghost touches | Restart; clean screen; remove screen protector; replace digitizer |
| **Damaged ports** | Bent pins, debris | Clean with soft brush; replace port if pins are broken |
| **Malware** | Suspicious apps, pop-ups, battery drain | Safe mode; uninstall suspect apps; antivirus scan; factory reset |
| **Cursor drift / touch calibration** | Software glitch or bad screen protector | Reboot; remove screen protector; use calibration tool; update OS |
| **Cannot install apps** | Low storage or MDM policy restriction | Free up storage; check MDM settings |
| **Stylus not working** | Damaged tip, dead battery, firmware issue | Inspect tip; check battery; update firmware |
| **Degraded performance** | Too many apps, low storage, outdated OS | Restart; clear cache; free storage; update OS |

---

## 5.5 Network Troubleshooting

| Symptom | Cause | Fix |
|---------|-------|-----|
| **Intermittent Wi-Fi** | Signal strength, interference, outdated drivers | Move closer to router; use Wi-Fi analyzer; switch to channels 1, 6, or 11 |
| **Slow network speeds** | Bandwidth hogs, congestion, old hardware, malware | Run speed test; restart router; configure QoS; upgrade hardware |
| **Limited connectivity** | DHCP failure, IP conflict, bad gateway/DNS | `ipconfig /release` → `ipconfig /renew`; verify gateway/DNS; swap cable |
| **Jitter** | Congestion, buffer bloat, poor ISP routing | Run latency test; use wired connection; enable QoS |
| **Poor VoIP quality** | Latency, jitter, packet loss, NAT/firewall issues | Test internet; configure QoS for voice traffic |
| **Port flapping** | Faulty port, bad cable, duplex mismatch | Move to different port; replace cable; match duplex settings |
| **High latency** | Congestion, distance, interference, old hardware | `ping` test; switch to wired (LAN); contact ISP |
| **External interference** | RF noise from neighboring networks/devices | Use 5 GHz; relocate router; switch channels; use LAN |
| **Authentication failures** | Wrong password, expired/locked account, time sync | Double-check credentials; forget and reconnect |
| **Intermittent LAN internet** | Loose cables, ISP issues, router overheating, DHCP lease | Check physical connections; power cycle modem/router; contact ISP |

### Ping Latency Reference
| Latency | Quality |
|---------|---------|
| 0–30 ms | Excellent — competitive gaming |
| 30–70 ms | Good — casual gaming/streaming |
| 70–100 ms | Average — acceptable for browsing |
| 100–150 ms | Fair — noticeable lag in real-time apps |
| 150ms+ | Poor — significant delays/buffering |

---

## 5.6 Printer Troubleshooting

| Symptom | Common Causes | Fix |
|---------|--------------|-----|
| **Lines on printed pages** | Dirty printhead/roller, low toner, worn drum | Run cleaning cycle; clean printhead; replace toner or drum |
| **Garbled print** | Wrong/outdated driver, corrupted job, language mismatch | Update/reinstall driver; clear print queue; verify printer language |
| **Paper jams** | Incorrect paper, dirty rollers, overloaded tray | Power off; remove jammed paper; clean/replace rollers |
| **Faded prints** | Low toner/ink, dried ink, fuser issue | Increase print quality; replace cartridge; inspect fuser |
| **Paper not feeding** | Worn rollers, foreign objects, wrong paper type | Clean rollers; reload paper; confirm paper type |
| **Multipage misfeed** | Worn separation pad, dirty rollers, humidity | Use correct paper; replace separation pads; replace feed rollers |
| **Multiple pending jobs** | Frozen print queue, spooler crash, offline printer | Cancel all jobs; restart Print Spooler (`services.msc`); reboot printer |
| **Speckling on pages** | Leaking cartridge, debris, dirty drum | Shake toner cartridge; clean interior; replace defective parts |
| **Double / echo images** | Residual image on drum, fuser malfunction | Check drum for buildup; verify fuser temp; replace faulty parts |
| **Grinding noise** | Worn rollers, foreign objects, misaligned carriage/gears | Power off; inspect and remove obstructions; service if needed |
| **Finishing issues** | Stapler/hole-punch problems | Empty hole-punch waste bin; adjust settings via printer software |
| **Wrong page orientation** | Incorrect driver or app setting | Correct orientation in driver; use Print Preview before printing |
| **Tray not recognized** | Dirty sensor, wrong settings, unseated tray | Reseat tray; clean sensors; verify printer settings; hard reset |
| **Connectivity issues** | Cable unplugged, wrong subnet, IP conflict | Check connections; verify IP; restart devices; `ping [printer IP]` |
| **Frozen print queue** | Corrupted job, spooler crash | Cancel jobs; restart Print Spooler; delete spool files at `C:\Windows\System32\spool\PRINTERS` |

---

*End of CompTIA A+ Core 1 (220-1201) Study Notes*
