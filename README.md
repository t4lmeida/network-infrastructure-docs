# 🌐 Industrial Infrastructure Migration & Network Engineering Docs

![Network Topology](diagrams/network-topology.png)

## 📌 Executive Summary

This repository documents the complete physical and logical network infrastructure design, deployment, and migration for a new industrial facility (90+ network drops). 

The primary business directive was to execute a seamless, site-to-site operational transition **without stopping production or business operations**, maintaining high availability for core ERP, File Server, and Active Directory services.

---

## 🎯 Key Business & Operational Metrics

- **Zero Downtime:** 0 minutes of user/operational downtime during site-to-site migration.
- **100% Uptime:** Continuous, uninterrupted network availability post-launch.
- **Cost Reduction:** Modernized legacy telephony by migrating 100% to **VoIP**, reducing telecom expenses by 10% and converting variable costs into predictable fixed rates..
- **High Performance:** Implemented end-to-end 1 Gbps Gigabit connectivity across all physical network drops.
- **Resilience:** Dual ISP setup with automated **Failover** to ensure Internet and Cloud service continuity.

---

## 🛠️ Architecture & Technical Stack

### **Physical Infrastructure & Cabling**
- **Rack Structure:** 44U Floor Cabinet with structured Patch Panel mappings, organized uplinks, and horizontal cable management.
- **End-to-End Gigabit Network:** Optimized cabling and patch panel distribution prioritizing critical operational sectors.

### **Logical Network & Services**
- **Site-to-Site Connectivity:** Configured a secure **WireGuard VPN** tunnel on Linux to seamlessly connect the legacy site to the new facility, enabling low-latency access to the ERP (Delphi/Database), Active Directory, and File Servers.
- **Core Network Routing:** Deployed a dedicated Linux server running `dhcpd` and custom gateway routing to bypass ISP router limitations.
- **Isolations & Virtualization:** Containerized the UniFi Ubiquiti Controller using **Podman + MongoDB** on Ubiquiti OS Server for centralized AP/Switch management.
- **Telephony Transformation:** Eliminated legacy analog lines and deployed 100% VoIP telephony.

---

## 📁 Repository Structure

```

├── README.md                          # Main documentation
├── diagrams/
│   └── rack_diagram.png               # Exported rack & network topology diagram
└── data/
    └── networking_mapping/            # Sanitized port mapping
```

---

## 👨‍💻 Author

**Thiago Oliveira Almeida**  
*IT Analyst | Data Science Undergraduate | Cloud & DevOps Enthusiast*  
- **LinkedIn:** (https://www.linkedin.com/in/thiago-almeida-37b560b2/)
- **Email:** t4lmeida@gmail.com
- **Whatsapp:** 37991159492  
- **Languages:** Portuguese (Native), English (Advanced), Spanish (Advanced)
