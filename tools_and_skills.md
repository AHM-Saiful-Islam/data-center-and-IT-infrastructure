# 🏗️ Data Center Technician — Tools & Equipment

A curated reference of software platforms, hardware tools, and physical equipment used in day-to-day data center operations — covering colocation environments, hyperscale facilities, and remote hands workflows.

> Based on hands-on experience at **Equinix Frankfurt** and **Digital Realty Frankfurt**, working under strict SLAs, 24/7 operational standards, and enterprise security protocols.

---

## 🖥️ Out-of-Band Server Management

Tools used for remote server access, hardware health monitoring, power control, and BIOS/firmware configuration — without requiring the operating system to be running.

- **iDRAC (Integrated Dell Remote Access Controller)** — Dell's OOB management interface. Used for power cycling, SOL (Serial Over LAN) console access, hardware health monitoring, and firmware updates on Dell PowerEdge servers.
- **iLO (Integrated Lights-Out)** — HP/HPE equivalent to iDRAC. Provides remote console, fan/temperature monitoring, and server lifecycle management on HP ProLiant servers.
- **IPMI (Intelligent Platform Management Interface)** — Vendor-neutral OOB standard. Used for remote power control, sensor data, and system event log (SEL) access across mixed-vendor environments.

---

## 📋 Ticketing & Incident Management

- **ServiceNow** — Primary ITSM platform for logging, tracking, and resolving incidents, change requests, and work orders. Used for remote hands tickets, cross-connect requests, asset updates, and SLA tracking in colo environments.

---

## 📊 DCIM & Infrastructure Monitoring

Tools for monitoring data center assets, power capacity, environmental conditions, and infrastructure documentation.

- **DCIM Platforms (e.g., Vertiv Trellis, Nlyte, Sunbird)** — Used for real-time power monitoring, capacity tracking, rack-level asset documentation, and environmental sensor management.
- **BMS (Building Management System)** — Monitors facility-level systems including HVAC, cooling units, UPS, and fire suppression. Integrated with DCIM for full operational visibility.
- **PDU Monitoring Interfaces** — Web-based dashboards on intelligent PDUs for per-outlet power metering, threshold alerts, and remote switching.

---

## 🔌 Cabling & Connectivity Tools

### Hardware
- **OTDR (Optical Time Domain Reflectometer)** — Fiber optic testing tool for identifying faults, measuring signal loss, and verifying splice quality on single-mode and multimode fiber runs.
- **Fiber Optic Cleaning Kit** — Ferrule cleaners, end-face inspection microscopes, and IPA swabs. Essential before any fiber connection to prevent signal degradation.
- **Ethernet Cable Crimper & RJ45 Connectors** — For terminating and repairing copper Cat6a/Cat8 patch cables.
- **Cable Tester (e.g., Fluke Networks)** — Validates continuity, wiring pinout, and signal integrity on copper and fiber runs.
- **Tone Generator & Probe Kit** — Traces cables through patch panels, raised floors, and overhead trays.
- **Label Maker (e.g., Brother PT series)** — For end-to-end cable labelling, rack labelling, and cross-connect documentation per facility standards.

### Software
- **Wireshark** — Network protocol analyzer for packet-level troubleshooting on live infrastructure.

---

## 🧰 Hardware & Break/Fix Toolkit

Tools used for rack & stack, component-level replacement, and server break/fix operations.

### Physical Tools
- **Screwdriver Set (Phillips, Flathead, Torx T8/T10/T20)** — Essential for server chassis, rack rails, and component access across Dell, HP, and Supermicro hardware.
- **Anti-Static Wrist Strap & ESD Mat** — Mandatory when handling sensitive components: RAM, NIC cards, SSDs, HDDs. Prevents electrostatic discharge damage.
- **Precision Tool Kit** — For handling delicate components in dense blade servers or 1U form factors.
- **Flashlight / Headlamp** — For working in poorly lit rack environments, especially in active hot aisles.
- **Magnetic Parts Tray** — Holds screws and small components during rack or chassis work.
- **Torque Screwdriver** — For consistent fastening on rack-mount equipment per vendor spec.

### Components Handled
- SSD, HDD (SAS/SATA/NVMe) — Hot-swap and cold-swap replacements
- NIC cards (1GbE, 10GbE, 25GbE) — PCIe installation and cabling
- DDR4 / DDR5 RAM — DIMM slot identification, seating, and POST verification
- PSU (Power Supply Units) — Hot-swap replacement in redundant power configurations
- Server rail kits — Rack mounting of 1U/2U/4U chassis for Dell, HP, Supermicro

---

## 🌡️ Environment & Safety Tools

- **Temperature & Humidity Monitor** — Handheld or rack-mounted sensors for spot-checking hot/cold aisle conditions and verifying ASHRAE compliance.
- **Multimeter** — Measures voltage and continuity on power circuits, PDUs, and cabling during troubleshooting.
- **Non-Contact Voltage Tester** — Safe identification of live circuits before working near power infrastructure.
- **Airflow Indicator (smoke pencil / anemometer)** — Verifies hot/cold aisle containment integrity and identifies bypass airflow issues.

---

## 📁 Documentation & Asset Management

- **Excel / Google Sheets** — Rack elevation diagrams, IP address management (IPAM), cable schedules, and asset inventories.
- **Visio / draw.io** — Network topology diagrams and physical infrastructure layout documentation.
- **Confluence** — Internal knowledge base for SOPs, runbooks, and change documentation.
- **Facility DCIM Portal** — Customer-facing asset portals used in colo environments (e.g., Equinix IBX, Digital Realty Fabric) for cross-connect ordering and remote hands ticket management.

---

## 🔐 Physical Security Tools & Systems

- **Access Control Systems (badge + PIN + biometric)** — Standard multi-factor entry for data halls, cages, and sensitive areas.
- **CCTV Monitoring** — Reviewed during incident investigations; awareness of camera coverage zones is part of operational protocol.
- **Visitor Escort Procedures** — Logging and escorting third-party vendors and customers within secure areas per facility policy.

---

## 🖧 Basic Network & System Tools

- **SSH Clients (PuTTY, MobaXterm)** — Terminal access to network devices and Linux servers for basic configuration and health checks.
- **Linux CLI** — Used for system status checks, log review, and basic configuration tasks (`ping`, `traceroute`, `ip`, `df`, `top`, `journalctl`).
- **Windows Server (RDP)** — Remote Desktop Protocol access for Windows-based infrastructure management.
- **IP Scanner (e.g., Angry IP Scanner, Advanced IP Scanner)** — Network device discovery and connectivity verification.

---

> 💡 **Tip:** In colo environments like Equinix and Digital Realty, always verify the customer's work order in ServiceNow before touching any equipment. Remote hands work is SLA-driven — documentation and communication are as critical as the physical task.

> ⚠️ **Safety Note:** Always follow site-specific ESD, PPE, and lockout/tagout (LOTO) procedures. In live data center environments, mistakes have operational and financial consequences for customers.

> 📌 **Scope:** This list reflects L1–L2 data center operations. Facility-specific tools and platforms may vary by operator (Equinix, Digital Realty, NTT, CyrusOne, etc.).
