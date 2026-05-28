# network-ports

A curated collection of common TCP/UDP ports used by internal infrastructure, Linux servers, routers, cameras, web services, and other high-value network targets.

Designed for:
- Network reconnaissance
- Infrastructure auditing
- Pentesting
- Service fingerprinting
- Fast `nmap` profiling
- Red team initial enumeration

---

# Features

- Categorized port lists
- TCP and UDP separation
- Ready-to-use `nmap` syntax
- Router vendor profiles
- Camera/DVR/NVR profiles
- Web service ports
- Internal enterprise service ports
- Linux infrastructure ports
- Copy-paste friendly formatting

---

# Included Categories

## Internal Servers

Common enterprise infrastructure services:

- SMB
- LDAP
- Kerberos
- MSSQL
- PostgreSQL
- Docker
- Kubernetes
- VMware
- Elasticsearch
- RabbitMQ
- WinRM
- NFS
- Redis
- MongoDB

---

## Linux Servers

Focused on Linux administration and infrastructure:

- SSH
- Docker API
- NFS
- Redis
- Kubernetes
- Prometheus
- Elasticsearch
- Webmin
- Node Exporter

---

## HTTP / Web Services

Common HTTP administration and application ports:

- 80
- 8080
- 8443
- 8888
- 9090
- 10000
- Kibana
- WebLogic
- Jupyter
- Alternate admin panels

---

## IP Cameras / DVR / NVR

Includes common ports for:

- RTSP
- ONVIF
- Dahua
- XMeye/Xiongmai
- Embedded web panels
- Vendor streaming services
- Discovery protocols

---

## Router Profiles

Vendor-specific profiles included:

- TP-Link
- Cisco
- MikroTik
- Ubiquiti / UniFi

Generic router/service discovery profiles are also included.

---

# Example Usage

## TCP Scan

```bash
nmap -sT -Pn -p 22,80,443,445,3389 <TARGET>
```

## UDP Scan

```bash
sudo nmap -sU -Pn -p 53,123,161,1900 <TARGET>
```

## Mixed TCP/UDP Scan

```bash
sudo nmap -sSU -Pn -p T:22,80,443,U:53,161 <TARGET>
```

## Service Detection

```bash
nmap -sV -sC <TARGET>
```

---

# Repository Structure

```text
network-ports/
├── internal-servers.txt
├── linux-servers.txt
├── http-ports.txt
├── cameras.txt
├── tplink.txt
├── cisco.txt
├── mikrotik.txt
├── ubiquiti.txt
├── generic-routers.txt
└── README.md
```

---

# Goals

This repository aims to provide:

- Fast reconnaissance references
- Reusable port profiles
- Practical enumeration shortcuts
- Cleaner workflow for infrastructure assessments

---

# Future Additions

Possible future categories:

- ICS / SCADA
- Industrial PLCs
- NAS devices
- Hypervisors
- VoIP systems
- PBX servers
- Cloud infrastructure
- Kubernetes exposure profiles
- IoT devices
- Smart home devices

---

# Contributing

Pull requests are welcome.

You can contribute:

- New vendor profiles
- Additional infrastructure ports
- Better `nmap` presets
- ICS/SCADA profiles
- Cloud infrastructure profiles
- IoT device profiles

---

# Disclaimer

This repository is intended for:

- Defensive security
- Authorized penetration testing
- Research
- Educational purposes

Only scan systems you own or are explicitly authorized to assess.

---

# License

MIT License
