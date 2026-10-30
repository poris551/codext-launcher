# Codext Launcher - IntelliJ Plugin

![Version](https://img.shields.io/badge/version-1.1.18-blue.svg)
[![IntelliJ IDEA](https://img.shields.io/badge/IntelliJ%20IDEA-2024.2+-orange.svg)](https://www.jetbrains.com/idea/)

> [!IMPORTANT]
> This version has been modified to launch [Loongphy/codext](https://github.com/Loongphy/codext) using the `codext` command instead of `codex`.

<img width="800" alt="The screenshot of Codex Launcher." src="https://github.com/user-attachments/assets/4ee3fbd8-e384-4672-94c6-e4e9041a8e0d" />

Codext Launcher is an **unofficial** IntelliJ IDEA launcher for [Codext](https://github.com/Loongphy/codext), based on [Codex Launcher](https://github.com/x0x0b/codex-launcher).

> **Important:** Install [Codext](https://github.com/Loongphy/codext) separately before using this plugin: `npm i -g @loongphy/codext`.

## Changes in 1.1.18

- Changed the terminal launch command from `codex` to `codext` to use Loongphy/codext.
- Preserved existing CLI arguments, including the `notify` callback for IDE refresh and completion notifications.
- Renamed the README display title to **Codext Launcher**. IDE action, settings, and terminal tab labels still use **Codex**.

> **For Windows users:** Please select your terminal shell in the plugin settings to ensure proper functionality. Go to _Settings (→ Other Settings) → Codex Launcher_.

## ✨ Features

- **One-click launch** from the toolbar or Tools menu
- **Integrated terminal** that opens a dedicated "Codex" tab in the project root
- **Completion notifications** after Codex CLI finishes processing the current run
- **Automatic file opening** for files updated by Codex
- **Built-in MCP server pairing** with guided setup for IntelliJ's MCP server (2025.2+)
- **Flexible configuration** for launch modes, models, and notifications

## 🛠️ Installation

### Prerequisites
- IntelliJ IDEA 2024.2 or later (or other compatible JetBrains IDEs)
- Codext installed and the `codext` command available in your terminal shell

### Installation
Build this modified checkout, then select **Settings → Plugins → ⚙ → Install Plugin from Disk** and choose `build/distributions/codex-launcher-1.1.18.zip`.

## 🚀 Usage

### Quick Start
1. Click the **Launch Codex** button in the main toolbar.
2. Or choose **Tools** → **Launch Codex**.
3. The integrated terminal opens a new "Codex" tab and runs `codext` automatically with the configured CLI arguments.

### Configuration
Open **Settings (→ Other Settings) → Codex Launcher** to pick the launch mode, model, notification behavior, and auto-open options.

## 📝 Development

### Building from Source
```bash
./gradlew buildPlugin
```

## 📄 License

This project is licensed under the terms specified in the [LICENSE](LICENSE) file.
