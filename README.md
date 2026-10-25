# 🦉 OChain

<p align="center">
  <img src="https://img.shields.io/badge/Platform-Linux-0a0c10?style=flat-square"/>
  <img src="https://img.shields.io/badge/Category-OAttack%20/%20Offensive-blue?style=flat-square"/>
  <img src="https://img.shields.io/badge/License-MIT-green?style=flat-square"/>
  <img src="https://img.shields.io/badge/Part%20of-OwlSec%20Toolkit-7b5ea7?style=flat-square"/>
  <img src="https://img.shields.io/badge/Version-1.0-cyan?style=flat-square"/>
</p>

> **OChain** — Advanced Propagation & BAS Simulation Engine ║

---

> ⚠️ **AUTHORISED USE ONLY** — Use only on systems you own or have explicit written permission to test. Unauthorised use is illegal.

---

## 📌 Overview

OChain is a safe propagation and breach-and-attack-simulation engine for purple-team and threat-emulation work. It discovers propagation paths, maps MITRE ATT&CK coverage, highlights credential-exposure and lateral-movement indicators and validates network segmentation — all non-destructively, with zero exploitation and zero real authentication. Safety guards restrict it to private/loopback targets and require explicit operator authorisation, and all artifacts are benign, timestamped and auto-cleaned.

---

## ✨ Features

- Non-destructive propagation-path discovery and lateral-movement indicators
- MITRE ATT&CK coverage mapping and expected-detection checklist export
- Credential-exposure and network-segmentation validation
- Safety guards: private/loopback targets only, explicit authorisation required
- TCP connectivity scan with banner grabbing and DNS resolution
- Dry-run planning and report export to JSON, CSV, HTML and XML

---

## ⚙️ Requirements

- **Linux**
- **No Python installation needed** — runs as a standalone executable

---

## 🚀 Usage

```bash
./OChain
./OChain --module scan --target 127.0.0.1 --ports 22,80,443 --yes
./OChain --dry-run --formats json,html
./OChain --help
```

---

## 📦 Part of OwlSec Toolkit

This tool is part of the **OwlSec** suite — a collection of 300+ security and privacy tools.

🔗 [owlsec.org](https://owlsec.org)

---

## ©️ License

MIT License — © Khaled S. Haddad

*Tools are distributed as pre-built executables. Source code is proprietary.*
