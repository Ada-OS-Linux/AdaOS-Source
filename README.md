# Ada OS

[![License: GPL‑3.0](https://img.shields.io/badge/License-GPLv3-blue.svg)](LICENSE)  

**Ada OS | Source** — The official source code for Ada OS Linux.

---

## Table of Contents

- [What Is Ada OS](#what-is-ada-os)  
- [Features](#features)  
- [Getting Started](#getting-started)  
  - [Prerequisites](#prerequisites)  
  - [Cloning the Repo](#cloning-the-repo)  
  - [Building Ada OS](#building-ada-os)  
- [Directory Structure](#directory-structure)  
- [Contributing](#contributing)  
- [License](#license)  
- [Resources](#resources)

---

## What Is Ada OS

Ada OS is a Linux-based operating system that provides a live‑build image with custom theming, tools, and services. It supports installation via a desktop environment and is designed for users who want a mix of stability, modern UI, and customizability. The source repo holds all the components needed to build the live image.

---

## Features

- Live build system for creating ISO images  
- Custom splash screen, icons, and themes included  
- Bootloader support (Syslinux, Isolinux, etc.)  
- Preconfigured hooks and services to provide out-of-the-box usability  
- GPL‑3.0 licensed — fully open source  

---

## Getting Started

### Prerequisites

Before building Ada OS from source, ensure you have:

- A Debian‑based distribution (or system with compatible tooling)  
- Root or sudo access  
- The following packages installed:  
  ```bash
  sudo apt install -y live-build squashfs-tools syslinux-common syslinux-utils xorriso isolinux git curl
  ```

### Cloning the Repository

```bash
git clone https://github.com/Ada-OS-Linux/AdaOS-Source.git
cd AdaOS-Source
```

### Building Ada OS

Once inside the project directory, you can build the live image by running:

```bash
sudo ./build
```

This should generate the ISO (or other live media) based on the configuration and assets in the repo.

---

## Directory Structure

Here’s a breakdown of important folders and what they contain:

| Directory | Purpose |
|-----------|---------|
| `.github/workflows` | CI/CD or build automation workflows. |
| `Services` | Custom services used by Ada OS. |
| `bootloaders` | Bootloader configurations. |
| `calamares` | Installer setup (if using Calamares). |
| `hooks` | Scripts/hooks that run during build/live boot. |
| `icons` | Icon sets used in the desktop environment. |
| `livebuild` | Configuration for live system builds. |
| `skel` | Skeleton/home templates for new users. |
| `sources` | Upstream source packages, overlays, or modifications. |
| `splash` | Splash screen images / boot graphics. |
| `themes/Lavanda-Sea-Dark` | Custom theme “Lavanda Sea Dark.” |

---

## Contributing

We welcome contributions! If you’d like to help, here are a few ways to get involved:

1. **Report Issues** — If you find bugs, missing features, or anything unexpected, open an issue.  
2. **Submit Pull Requests** — For fixes, improvements, new themes, etc. Please follow the coding & style patterns already in the repo.  
3. **Design & Assets** — Help with icons, themes, splash screens improves the visual polish.  
4. **Documentation** — Better docs (install guides, usage examples, etc.) are always helpful.

Before contributing, please read the [License](#license) to make sure your contributions are compatible.

---

## License

This project is licensed under **GPL‑3.0**. See the [LICENSE](LICENSE) file for details.

---

## Resources

- **Download latest builds** — from the GitHub Actions workflow: build_monthly.  
- **Mirror / alternate source** — `source.adaoslinux.xyz`  
- **Community & Contact** — Use GitHub Issues for bugs and feature requests.  

---

*Ready to build your own custom Ada OS? Let’s get started!*  
