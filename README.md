**Junior Cybersecurity Engineer** · 3rd-year Cybersecurity Engineering student · CompTIA Security+

I'm after the whole field: how systems are built, how they get broken into and how all of that gets caught. Right now I'm deep in the defensive end, building a SOC lab from scratch. Breaking into it properly is next.

#### Currently building: SOC Automation Lab

A university team project about alert fatigue. The target is to take ~1,000 raw alerts, deduplicate, group and enrich them, and leave an analyst with ~10 incidents that actually need a human.

```text
Wazuh + Suricata  →  Shuffle (SOAR)  →  Cortex + MISP  →  scoring & dedup  →  TheHive
```

I built the lab and keep it running:

- **Network:** a Proxmox host behind OPNsense, with separate VLANs for victims, SOC tooling and the attacker box, and WireGuard access for the team.
- **Telemetry:** Wazuh agents on an AD domain controller, Windows workstations, a Linux web server and the firewall itself. Sysmon on every Windows host, Suricata alerts going through the same pipeline.
- **Detection testing:** a deliberately vulnerable web app that we attack from Kali to see what gets caught. First finding: a webshell run from the upload folder raised no alert at all. Custom rule in progress.

Installing the tools was the easy part. The real work was figuring out why one workstation had never been sending its Sysmon logs, and why two others live six hours in the future.

→ [soc-automation-lab](https://github.com/ORG-OR-USER/soc-automation-lab)

#### Toolbox

| Area | Tools |
|---|---|
| Detection & logging | Wazuh · Suricata · Sysmon |
| Response & threat intel | Shuffle · TheHive · Cortex · MISP |
| Infrastructure | Proxmox VE · OPNsense · Active Directory · Linux · Docker |

#### Off-screen

Urban exploration: abandoned factories, old hospitals, a headlamp and a camera. I call it physical recon.

<sub>Find me on [LinkedIn](https://www.linkedin.com/in/antonich2508/). Always happy to talk detection engineering, home labs or a good abandoned building.</sub>

