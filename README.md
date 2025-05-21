# DWM Config 

This repository contains my custom configuration for [DWM (Dynamic Window Manager)](https://dwm.suckless.org/), along with related tools including `dmenu`, `st` (Simple Terminal), and `slstatus`. It's a minimalist and performance-focused window management setup for X11.

---

## 📁 Repository Structure

- `dwm/` – Customized DWM build with personal patches and configuration.
- `dmenu/` – Custom build of dmenu, a dynamic menu for X.
- `st/` – Patched version of st (Simple Terminal) with aesthetic and usability improvements.
- `slstatus/` – Lightweight status monitor for DWM.

---

## ✅ Features

- Lightweight and fast tiling window manager
- Custom keybindings and appearance tweaks
- Integrated system status bar (`slstatus`)
- Personalized and patched builds for improved workflow

---

## 🧰 Requirements

Before installing, ensure you have:

- `Xlib` development libraries (e.g., `libx11-dev`)
- `make` and `gcc`
- A POSIX-compatible environment (Linux/BSD)
- Fonts and terminal emulator (e.g., `xfontsel`, `xterm`)

---
## ⚙️ Installation

Clone this repository:

```bash
git clone https://github.com/Rogshivam/DWM-config.git
cd DWM-config
```
Build and install each component:

```bash
cd dwm
sudo make clean install
```
```bash

cd ../dmenu
sudo make clean install
```
```bash

cd ../st
sudo make clean install
```
```bash

cd ../slstatus
sudo make clean install
```
⚠️ These commands will install the binaries to /usr/local/bin. You may need to log out and log in again for changes to take effect.

🚀 Usage
To start DWM, ensure your .xinitrc file contains:

```bash

exec dwm

```
Then run:
```bash

startx
```
🛠 Customization
To customize any component:

Edit the config.h file inside the respective directory (dwm/, st/, etc.).

Rebuild using:

```bash

sudo make clean install
```
📝 License
This project is licensed under the MIT License. See the LICENSE file for details.

