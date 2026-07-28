# Ariadna

**Lightweight Network Discovery Tool for PDU Port & MAC Address Lookup**

![Status](https://img.shields.io/badge/status-beta-orange)
![Version](https://img.shields.io/badge/version-0.6.6-blue)
![License](https://img.shields.io/badge/license-MIT-green)

---

## Overview

Ariadna is a lightweight web tool that automates the discovery of switch ports and MAC addresses for Power Distribution Units (PDUs) in data center environments. It eliminates the need for engineers to physically navigate through a facility and connect directly to each PDU's web interface.

> Named after Ariadne of Greek mythology — the guide who helped navigate the Labyrinth.

---

## The Problem

When initially deploying managed PDUs, engineers face a critical limitation:

- **PDUs do not receive IPv6 addresses "out of the box"**
- Remote configuration is impossible
- Engineers must physically visit each rack, connect a laptop via patch cord, and manually search for links

This process results in:
- ⏱️ **Significant time loss**
- 🏃 **Physical strain**
- ⚠️ **Risk of human error**

---

## The Solution

Ariadna takes over the routine work, providing:

- 🔍 **Instant search** by switch name, inventory number, or FQDN
- 📊 **Clean results** — VLAN / Port / MAC table
- 📋 **One-click copy** for any value
- 📤 **Flexible export** in multiple formats
- 🌙 **Dark & Light** themes

---

## Features

| Feature | Description |
|---------|-------------|
| **Multi-switch Search** | Query multiple switches at once (space, comma, or semicolon-separated) |
| **Duplicate Tolerant** | Handles duplicate entries gracefully |
| **Extended MAC Pools** | Broad manufacturer identifier pool for PDUs |
| **Host Detection** | Finds hosts, switches, and consoles |
| **Export Tools** | Flexible result export configuration |
| **Zero Backend** | Works as a single HTML file |
| **Responsive UI** | Dark and light theme support |

---

## Quick Start

### Prerequisites

- A CORS-enabled browser extension (e.g., [Allow CORS](https://chromewebstore.google.com/detail/allow-cors-access-control/lhobafahddgcelffkeicbaginigeejlf) for Chromium-based browsers)

### Installation

1. **Install CORS extension** in your browser
2. **Download** `Ariadna-0.6.6.html`
3. **Open** the file in your browser

### Usage

1. Open `Ariadna-0.6.6.html`
2. Enter switch name, inventory number, or FQDN
3. (Optional) Select search mode or add custom MAC pool
4. Click **Search**
5. Copy results or export in your preferred format

---

### Tech Stack

| Layer | Technology |
|-------|------------|
| Frontend | HTML5, Tailwind CSS, Vanilla JavaScript |
| API Integration | RackTables (via curl requests) |
| UI/UX | Lightweight, intuitive interface |

---

## Security Fork: Miniadna

For enhanced security, a Tailwind-free fork is available:

**Miniadna** — All CSS is stored locally within the single HTML file, eliminating external framework dependencies and reducing potential attack surface.

📄 [Miniadna-0.1.html](./Miniadna-0.1.html)

> ⚠️ Minor rendering inconsistencies may occur in this version.

---

## Changelog

### v0.6.6 (June 25, 2026)

- ✅ Multi-switch array processing with duplicate tolerance
- ✅ Host, switch, and console search
- ✅ Extended standard MAC address pools
- ✅ Flexible result export tool
- ✅ Performance optimizations
- ✅ Tailwind-free fork created

---

## Roadmap

- [ ] Collect feedback and fix bugs
- [ ] IP detection and ping module for connected PDUs
- [ ] Expand beyond PDU search
- [ ] Deploy on internal hosting

---

## Requirements

| Requirement | Details |
|-------------|---------|
| Browser | Modern browser (Chrome, Firefox, Edge, Safari) |
| CORS Extension | Required for API queries |
| Network Access | Must have access to RackTables API |

---

## ⚠️ Known Limitations

- Requires CORS extension for API queries
- No internal hosting yet (standalone HTML file)
- No IPv6 support for direct PDU configuration

---

## License

MIT License

Copyright (c) 2026 felixred

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.


---

## Contributing

Contributions, issues, and feature requests are welcome!

---

*Made with ❤️ by [felixred](https://github.com/solidfab)*
