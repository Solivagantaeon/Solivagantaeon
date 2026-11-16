**Junior Cybersecurity Engineer** · 3rd-year Cybersecurity Engineering student

![CompTIA Security+](https://img.shields.io/badge/CompTIA-Security%2B-C8202F?style=flat-square&logo=comptia&logoColor=white)
![Now](https://img.shields.io/badge/now-security%20engineer-1f6feb?style=flat-square)
![Goal](https://img.shields.io/badge/goal-security%20architect-2ea043?style=flat-square)

I'm after the whole field: how systems are built, how they get broken into and how all of that gets caught. Right now I'm deep in the defensive end, building a SOC lab from scratch. Breaking into it properly is next.

#### Currently building: SOC Automation Lab

A side project I'm building with friends, aimed at alert fatigue. The target is to take ~1,000 raw alerts, deduplicate, group and enrich them, and leave an analyst with ~10 incidents that actually need a human.

```mermaid
flowchart LR
    A["Wazuh + Suricata<br/>~1,000 alerts"] --> B["Shuffle<br/>SOAR"]
    B --> C["Cortex + MISP<br/>enrichment"]
    C --> D["Scoring<br/>& dedup"]
    D --> E["TheHive<br/>~10 incidents"]
```

I built the lab and keep it running:

- **Network:** a Proxmox host behind OPNsense, with separate VLANs for victims, SOC tooling and the attacker box, and WireGuard access for the rest of the crew.
- **Telemetry:** Wazuh agents on an AD domain controller, Windows workstations, a Linux web server and the firewall itself. Sysmon on every Windows host, Suricata alerts going through the same pipeline.
- **Detection testing:** a deliberately vulnerable web app that we attack from Kali to see what gets caught.


→ [soc-automation-lab](https://github.com/ORG-OR-USER/soc-automation-lab)

#### Toolbox

| Area | Tools |
|---|---|
| Detection & logging | ![Wazuh](https://img.shields.io/badge/Wazuh-3595F3?style=flat-square) ![Suricata](https://img.shields.io/badge/Suricata-EF7D00?style=flat-square) ![Sysmon](https://img.shields.io/badge/Sysmon-0078D4?style=flat-square) |
| Response & threat intel | ![Shuffle](https://img.shields.io/badge/Shuffle-FF8544?style=flat-square) ![TheHive](https://img.shields.io/badge/TheHive-F3C500?style=flat-square) ![Cortex](https://img.shields.io/badge/Cortex-2E3A4D?style=flat-square) ![MISP](https://img.shields.io/badge/MISP-1A4C7A?style=flat-square) |
| Infrastructure | ![Proxmox](https://img.shields.io/badge/Proxmox%20VE-E57000?style=flat-square&logo=proxmox&logoColor=white) ![OPNsense](https://img.shields.io/badge/OPNsense-E44A20?style=flat-square&logo=opnsense&logoColor=white) ![WireGuard](https://img.shields.io/badge/WireGuard-88171A?style=flat-square&logo=wireguard&logoColor=white) ![Active Directory](https://img.shields.io/badge/Active%20Directory-0078D4?style=flat-square) ![Linux](https://img.shields.io/badge/Linux-333333?style=flat-square&logo=linux&logoColor=FCC624) ![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white) |
| Offense | ![Kali Linux](https://img.shields.io/badge/Kali%20Linux-557C94?style=flat-square&logo=kalilinux&logoColor=white) |

#### Off-screen
Urbex: abandoned factories and old hospitals, but also tunnels, rooftops and the kind of infrastructure most people only see from the outside.

<sub>Find me on [LinkedIn](https://www.linkedin.com/in/antonich2508/). Always happy to talk detection engineering, home labs or a good abandoned building.</sub>
