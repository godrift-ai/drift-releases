# Drift CLI

<div align="center">

**Your AI-Powered Copilot for Robotics Simulations**

[![Latest Release](https://img.shields.io/badge/version-1.0.17-blue.svg)](https://github.com/godrift-ai/drift-releases/releases/latest)
[![Platform](https://img.shields.io/badge/platform-Linux-lightgrey.svg)](https://github.com/godrift-ai/drift-releases/releases)
[![License](https://img.shields.io/badge/license-MIT-green.svg)](LICENSE)

[Website](https://godrift.ai) • [Issues](https://github.com/godrift-ai/drift-releases/issues) • [Docs](https://docs.github.com)

</div>

---

## 🚀 Quick Install

Get started with Drift CLI in seconds:

```bash
curl -fsSL https://godrift.ai/install | bash
```

**That's it!** Once installed, simply run `drift` to start.

---

## 📦 Latest Release

**Current Version:** `1.0.17` ([View Release Notes](https://github.com/godrift-ai/drift-releases/releases/latest))

Download the `.deb` package directly:
- [drift-cli_1.0.17_amd64.deb](https://github.com/godrift-ai/drift-releases/releases/latest)

---

## What is Drift?

Drift CLI eliminates the steep learning curve of robotics simulation development. It's an AI-powered assistant that understands natural language and helps you build, test, and debug complex robotic systems using conversational commands.

**No more wrestling complex ROS2 commands or Gazebo configurations** — just describe what you want to build, and Drift handles the rest.

### ✨ Key Features

- **🗣️ Natural Language Interface** — Talk to your simulation like you're talking to a colleague
- **🤖 ROS2 & Gazebo Integration** — Seamless workflow with your favorite robotics tools
- **⚡ Intelligent Workspace Management** — Automatic package and workspace generation
- **🔄 Adaptive Planning** — Real-time error recovery and problem-solving
- **📄 Launch File Generation** — Automatic creation and validation of launch files
- **🎯 Process Management** — Track and manage multiple background processes
- **📊 Smart Debugging** — AI-assisted troubleshooting and error analysis

### 💡 Example Commands

```bash
drift> create a three arm manipulator with camera sensor
drift> launch my robot with the custom world file
drift> add a lidar sensor to my robot and rebuild
drift> why isn't my camera publishing images?
```

---

## 🖥️ System Requirements

- **OS:** Ubuntu 20.04+ (Debian-based distributions)
- **ROS:** ROS2 (Humble, Foxy, or later recommended)
- **Gazebo:** Gazebo Sim (Harmonic)
- **Architecture:** x86_64 (amd64)

We are bring support for older versions of ROS and Gazebo as well

---

## 📚 Getting Started

### 1. Install Drift CLI

```bash
curl -fsSL https://godrift.ai/install | bash
```

### 2. Launch Drift

```bash
drift
```

### 3. Start Building

```
drift> /help                    # View all commands
drift> /version                 # Check your version
drift> create a ROS workspace   # Start building!
```

### 4. Special Commands

- `/help` — Show comprehensive help and examples
- `/version` — Display version information
- `/update` — Update to the latest version
- `/ps` — Show running background processes
- `/clear` — Clear the terminal screen
- `/exit` — Exit Drift CLI

---

## 🔄 Updates

Drift CLI includes automatic update detection. When a new version is available, you'll see a notification on startup like this:

```
ℹ️  A new version (1.1.0) is available. Type /update to install.
```

Simply run:
```bash
drift> /update
```

---

## 🛠️ Manual Installation

If you prefer to install manually:

1. Download the latest `.deb` package from [Releases](https://github.com/godrift-ai/drift-releases/releases/latest)
2. Install with dpkg:
   ```bash
   sudo dpkg -i drift-cli_*.*.*_amd64.deb
   ```
3. Run `drift` to start

---

## 🐛 Troubleshooting

### Issue: "Command not found: drift"
**Solution:** Try restarting your terminal or running:
```bash
source ~/.bashrc  # or ~/.zshrc
```

### Issue: Update fails
**Solution:** Manually download and install the latest `.deb` package from the releases page.

### Issue: Permission denied errors
**Solution:** Ensure you have proper permissions. The installer may need sudo access.

---

## 💬 Support & Community

- **🐛 Found a bug?** [Report it here](https://github.com/godrift-ai/drift-releases/issues)
- **💡 Have a feature request?** [Let us know](https://github.com/godrift-ai/drift-releases/issues/new)
- **📖 Need help?** Run `drift --help` or email at founders@godrift.ai
- **🌐 Website:** [godrift.ai](https://godrift.ai)

---

## ❤️ Made with Love for the Robotics Community

Drift was born out of a simple observation: **robotics development is incredibly powerful but unnecessarily complex**. We've spent countless hours wrestling with ROS configurations, debugging launch files, and searching through documentation just to get simple things working.

**We built Drift because we believe robotics should be accessible to everyone** — from students taking their first steps into ROS, to experienced engineers who just want to move faster.

This tool is our gift to the robotics community. We hope it saves you time, reduces frustration, and lets you focus on what really matters: **building amazing robots**.

Whether you're:
- 🎓 A student learning ROS for the first time
- 🔬 A researcher iterating on novel algorithms
- 🏭 An engineer developing production systems
- 🤖 A hobbyist bringing your robot dreams to life

**Drift is here to help you succeed.**

---

## 🙏 Acknowledgments

Drift CLI wouldn't be possible without the incredible open-source robotics community. Special thanks to:

- **ROS2** — For providing the foundation of modern robotics
- **Gazebo** — For powering realistic simulations
- **The entire robotics community** — For pushing the boundaries of what's possible

---

## 📄 License

Drift CLI is released under the [MIT License](LICENSE).

---

## 🚀 What's Next?

We're continuously improving Drift CLI based on your feedback. Check our [releases page](https://github.com/godrift-ai/drift-releases/releases) to see what's new, and don't hesitate to reach out with suggestions.

**Happy building! 🤖**

---

<div align="center">

**[Get Started](https://docs.godrift.ai)** • **[View Releases](https://github.com/godrift-ai/drift-releases/releases)** • **[Get Support](https://github.com/godrift-ai/drift-releases/issues)**

Made with ❤️ by the Drift team

</div>
