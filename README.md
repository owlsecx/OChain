<div align="center">

# 🦉 OChain

**Propagation & Breach Simulation Engine**

![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![MITRE ATT&CK](https://img.shields.io/badge/MITRE-ATT%26CK-red?style=for-the-badge)
![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)

*Part of the [OwlSec](https://owlsec.org) Toolkit*
```
██████╗  ██████╗██╗  ██╗ █████╗ ██╗███╗   ██╗
██╔═══██╗██╔════╝██║  ██║██╔══██╗██║████╗  ██║
██║   ██║██║     ███████║███████║██║██╔██╗ ██║
██║   ██║██║     ██╔══██║██╔══██║██║██║╚██╗██║
╚██████╔╝╚██████╗██║  ██║██║  ██║██║██║ ╚████║
 ╚═════╝  ╚═════╝╚═╝  ╚═╝╚═╝  ╚═╝╚═╝╚═╝  ╚═══╝
       Scan · Credentials · WMI · SSH · Obfuscation · Full Chain
```

</div>

---

## 📌 Overview

**OChain** is a safe propagation and breach simulation engine designed for **purple team exercises**. It validates network segmentation, detection coverage, and SSH/credential exposure — using only benign indicators with no real exploitation.

---

## 🖥️ Simulation Modules

| Option | Module | MITRE TTP | Description |
|--------|--------|-----------|-------------|
| `[1]` | Network Scan | T1046 | TCP connectivity discovery |
| `[2]` | Credential Indicators | T1078 / T1110 | Authentication indicators only — no actual auth |
| `[3]` | WMI Indicator | T1059 | Local execution simulation — benign commands only |
| `[4]` | SSH Key Check | T1021 | Local SSH permission inspection |
| `[5]` | Obfuscation | T1027 | Generate benign obfuscated artifact |
| `[6]` | Full Chain | All | Run all modules in sequence |

---

## 🛡️ MITRE ATT&CK Coverage

| TTP | Technique |
|-----|-----------|
| `T1046` | Network Service Discovery |
| `T1021` | Remote Services (connectivity only) |
| `T1078` | Valid Accounts (indicator only) |
| `T1110` | Brute Force (indicator only, no auth) |
| `T1059` | Command Interpreter (local benign) |
| `T1027` | Obfuscated Files (benign artifact) |

---

## ⚡ Scan Profiles

| Profile | Threads | Timeout | Jitter |
|---------|---------|---------|--------|
| `stealth` | 20 | 1.0s | 0.05 – 0.25s |
| `normal` | 60 | 0.8s | 0.01 – 0.10s |
| `noisy` | 120 | 0.6s | 0.00 – 0.03s |

---

## 🔒 Safety Policy

- Private and loopback networks only by default
- Requires explicit permission acknowledgement before running
- No authentication attempts — indicators only
- No remote execution — local benign commands only
- All artifacts are benign and auto-cleaned after simulation

---

## ⚙️ Requirements

- Linux (any distro)
- The tool is pre-built — no Python installation needed

---

## ⚠️ Legal Disclaimer

> **THIS TOOL IS FOR AUTHORIZED PURPLE TEAM EXERCISES ONLY.**  
> Must only be run on networks and systems you own or have explicit written permission to test.  
> Unauthorized use is illegal and unethical.  
> The developer is not responsible for any misuse.

---

## 📦 Part of OwlSec Toolkit

This tool is part of the **OwlSec** suite — a collection of 300+ security and privacy tools.

> 🔗 [owlsec.org](https://owlsec.org)

---

## ©️ License

MIT License — © Khaled S. Haddad

*Tools are distributed as pre-built executables. Source code is proprietary.*
