# 🎮 GameJoy - Retro Game Launcher

<div align="center">

![Version](https://img.shields.io/badge/version-1.0.0-blue.svg)
![License](https://img.shields.io/badge/license-MIT-green.svg)
![Electron](https://img.shields.io/badge/Electron-28.0.0-47848F.svg)
![Platform](https://img.shields.io/badge/platform-Windows-blue.svg)

**A modern, all-in-one retro game launcher built with Electron**

*Play PSP, Game Boy Advance, and Nintendo DS games from a single beautiful interface*

</div>

---

## ✨ Features

### 🎯 Multi-System Support
- **PlayStation Portable (PSP)** - Powered by PPSSPP
- **Game Boy Advance (GBA)** - Powered by mGBA
- **Nintendo DS (NDS)** - Powered by DeSmuME

### 🖥️ Modern Interface
- Clean, intuitive UI with smooth animations
- Interactive splash screen with credits
- System selector with navigation arrows
- Game library with visual grid layout
- Easy ROM file management

### ⚡ Key Features
- **Windows Desktop App** - Standalone executable, no installation required
- **Auto-Download** - Automatically downloads emulators when needed
- **Game Library** - Organize and launch your games easily
- **Full Keyboard Support** - Complete key bindings for all systems
- **Save States** - Save and load your game progress
- **Plug & Play** - Just add your ROM files and start playing

---

## 📥 Installation

### Simple 3-Step Process
1. Download the latest `GameJoy-v1.0.0-Windows-x64.zip` from the [Releases](../../releases) page
2. Extract the ZIP file to your preferred location
3. Run `GameJoy.exe` - No installation needed!

**System Requirements:**
- Windows 10 or Windows 11 (64-bit)
- 4GB RAM minimum
- Graphics card with DirectX 11 support

---

## 🎮 How to Use

### First Launch
1. Launch GameJoy
2. Click through the splash screen
3. Select your desired gaming system (PSP, GBA, or NDS)
4. The emulator will auto-download if not present

### Adding Games
1. Click **"Select Game"** or **"Add Game"** button
2. Browse to your ROM file (`.iso`, `.cso` for PSP | `.gba` for GBA | `.nds` for NDS)
3. The game will appear in your library
4. Click on a game to launch it

### Playing Games
- Use keyboard controls (see Key Bindings section below)
- Save states are automatically managed
- Close the game window to return to the launcher

---

## ⌨️ Key Bindings

### PlayStation Portable (PSP)
| PSP Button | Keyboard Key |
|-----------|-------------|
| D-Pad Up | `↑` Arrow Up |
| D-Pad Down | `↓` Arrow Down |
| D-Pad Left | `←` Arrow Left |
| D-Pad Right | `→` Arrow Right |
| ✕ (Cross) | `Z` |
| ○ (Circle) | `X` |
| □ (Square) | `A` |
| △ (Triangle) | `S` |
| L Trigger | `Q` |
| R Trigger | `W` |
| Start | `Enter` |
| Select | `Backspace` |
| Analog Stick | `I, K, J, L` |

### Game Boy Advance (GBA)
| GBA Button | Keyboard Key |
|-----------|-------------|
| D-Pad Up | `↑` Arrow Up |
| D-Pad Down | `↓` Arrow Down |
| D-Pad Left | `←` Arrow Left |
| D-Pad Right | `→` Arrow Right |
| A Button | `Z` |
| B Button | `X` |
| L Trigger | `A` |
| R Trigger | `S` |
| Start | `Enter` |
| Select | `Backspace` |

### Nintendo DS (NDS)
| NDS Button | Keyboard Key |
|-----------|-------------|
| D-Pad Up | `↑` Arrow Up |
| D-Pad Down | `↓` Arrow Down |
| D-Pad Left | `←` Arrow Left |
| D-Pad Right | `→` Arrow Right |
| A Button | `X` |
| B Button | `Z` |
| X Button | `A` |
| Y Button | `S` |
| L Trigger | `Q` |
| R Trigger | `W` |
| Start | `Enter` |
| Select | `Backspace` |
| Touchscreen | Mouse Click |

### Universal Emulator Controls
| Function | Key |
|---------|-----|
| Fast Forward | `Tab` |
| Save State | `F5` |
| Load State | `F7` |
| Screenshot | `F12` |
| Full Screen | `F11` or `Alt + Enter` |
| Pause/Resume | `Esc` |
| Increase Speed | `+` |
| Decrease Speed | `-` |
| Reset | `Ctrl + R` |

---


### Supported File Formats
- **PSP**: `.iso`, `.cso`, `.pbp`
- **GBA**: `.gba`
- **NDS**: `.nds`, `.zip`

---

## 🤝 Credits

### Created By
**Hein Htet Zaw (Rayy)**  
© 2026 GameJoy

### Powered By
- **[PPSSPP](https://www.ppsspp.org/)** - PlayStation Portable Emulator (GPL v2+)
- **[mGBA](https://mgba.io/)** - Game Boy Advance Emulator (MPL 2.0)
- **[DeSmuME](https://desmume.org/)** - Nintendo DS Emulator (GPL v2)
- **[Electron](https://www.electronjs.org/)** - Desktop Application Framework (MIT)

### Special Thanks
- All emulator developers and contributors
- The open-source gaming community
- Everyone who has contributed to retro gaming preservation

*See [CREDITS.txt](CREDITS.txt) for full license information*

---

## ⚖️ License

This project is licensed under the MIT License - see the LICENSE file for details.

**Note:** The bundled emulators (PPSSPP, mGBA, DeSmuME) retain their original licenses:
- PPSSPP: GPL v2+
- mGBA: Mozilla Public License 2.0
- DeSmuME: GPL v2

---

## ⚠️ Legal Notice

This launcher is for use with legally obtained game backups only. Users are responsible for ensuring they own physical copies of any games they play through this launcher. This project does not include or distribute any copyrighted game ROMs or BIOS files.

---

## 📞 Support

Found a bug or have a suggestion?
- Open an [Issue](../../issues)
- Submit a [Pull Request](../../pulls)

---

## 🌟 Star History

If you find GameJoy useful, please consider giving it a star ⭐

---

<div align="center">

**Made with ❤️ for the retro gaming community**

[Report Bug](../../issues) · [Request Feature](../../issues)

</div>

## Keyboard Controls

| Key | PSP Button |
|-----|-----------|
| Arrow Keys | D-Pad |
| W, A, S, D | Analog Stick |
| Space | Cross (X) |
| Z | Square |
| X | Triangle |
| C | Circle |
| Q | L Trigger |
| E | R Trigger |
| Enter | Start |
| Shift | Select |

## Integration with PSP Emulator Core

This is a UI framework. To integrate an actual PSP emulator:

1. **Add emulator core** - Integrate a PSP emulation library (e.g., PPSSPP core)
2. **Connect renderer.js** - Hook up the canvas rendering to the emulator
3. **Handle input** - Map keyboard events to emulator input
4. **Audio output** - Connect audio from emulator to Web Audio API
