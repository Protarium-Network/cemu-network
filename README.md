# Protarium Network Config for Cemu

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

Configuration file to connect [Cemu](https://cemu.info/) (Wii U emulator) to the **Protarium** network servers.

## 📋 What is this?

This repository contains the `network_services.xml` file that redirects Cemu's online services to [Protarium](https://protarium.lol) servers, enabling online functionality through the Protarium network.

## 🔧 Installation

### Automatic (recommended)

1. Download [`network_services.xml`](network_services.xml) from this repository
2. Place it in the root of your **Cemu installation folder** (next to `Cemu.exe`)
3. Launch Cemu — you should see **Protarium** displayed as the active network in the bottom-right corner

### Manual

1. Clone this repository:
   ```bash
   git clone https://github.com/Protarium-Network/cemu-network.git
   ```
2. Copy `network_services.xml` to your Cemu installation directory
3. Restart Cemu

## 🌐 Service Endpoints

| Service | Description | Endpoint |
|---------|-------------|----------|
| **ACT** (Account) | Account server & authentication | `account.protarium.lol` |
| **BOSS** (SpotPass) | Background data delivery | `api.protarium.lol` |
| **OLV** (Miiverse) | Miiverse social network | `disc.protarium.lol` |
| **ECS** | eShop services | Nintendo (default) |
| **NUS** | System & title updates | Nintendo (default) |
| **IAS** | Identity authentication | Nintendo (default) |
| **CCS** | Content download | Nintendo (default) |
| **IDBE** | Icon data | Nintendo (default) |
| **Tagaya** | Version list | Nintendo (default) |

> **Note:** Only the Protarium-specific services (ACT, BOSS, OLV) are redirected. Other services remain on Nintendo's default servers.

## ⚙️ Configuration Details

- **SSL Verification**: Disabled (`disablesslverification = 1`) — required for custom server connectivity
- **Network Name**: `Protarium` — displayed in Cemu's status bar

## 📁 File Structure

```
network_services.xml    # Place this in your Cemu root directory
```

## 🔗 Requirements

- [Cemu](https://cemu.info/) v2.0 or later (tested on v2.6)
- A Protarium account — visit [protarium.lol](https://protarium.lol) for more information

## 🤝 Contributing

Contributions are welcome! If endpoints change or new services are added, feel free to open a pull request.

## 📄 License

This project is licensed under the MIT License — see the [LICENSE](LICENSE) file for details.

## ⚠️ Disclaimer

This project is not affiliated with Nintendo or the Cemu development team. Use at your own risk. All trademarks are the property of their respective owners.

_Maintained by [noctis-nex](https://github.com/noctis-nex) as part of Protarium Network.
