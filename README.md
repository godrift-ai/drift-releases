# Drift Desktop

<div align="center">

**The platform for robotics simulation — from natural language to a running robot, in one place.**

[![Platform](https://img.shields.io/badge/platform-Linux-lightgrey.svg)](https://github.com/godrift-ai/drift-releases/releases)

[Website](https://godrift.ai) • [Docs](https://docs.godrift.ai) • [Issues](https://github.com/godrift-ai/drift-releases/issues)

</div>

---

## 🚀 Quick Install

One command installs the Drift Desktop app and its command-line companion, and launches the app for you when a display is available:

```bash
curl -fsSL https://godrift.ai/install | bash
```

That's it. When it finishes, the app opens; anywhere else you land in a terminal, typing `drift` gives you the same intelligence at the command line.

---

## What is Drift Desktop?

Drift Desktop is a purpose-built environment for people who build robots — a workspace that understands what a scene, an asset, a sensor, a controller and a run *are*, and lets you compose them by describing what you want rather than by memorising APIs across three simulators and half a dozen tools.

The everyday robotics stack — Gazebo worlds, MuJoCo scenes, Isaac Sim environments, launch files, controllers, calibration passes — is powerful and fragmented. Drift puts a single agent between you and all of it, so a sentence like *"give me an indoor kitchen, drop a Booster T1 in front of the counter, and start recording joint torques"* becomes an actual scene you can inspect, tweak and re-run.

---

## ✨ What Makes it Powerful

- **Talk-to-your-lab interface** — describe a robot, a task or a fix in plain language; Drift plans, builds, and runs it, showing you every step so you can steer or override.
- **Live 3D viewport** — meshes, sensors, contacts and trajectories render inline as the agent works. Nothing hides in a headless terminal.
- **Robot library** — curated humanoids, arms, quadrupeds and grippers you can drop into a scene by name, or bring your own URDF / MJCF / USD.
- **Scene understanding** — worlds are objects, not blobs of XML. Change lighting, swap the floor, add a shelf, and everything else keeps working.
- **Reproducible runs** — every session, every asset choice and every command is recorded, so a run that worked yesterday still works tomorrow — and you can share the exact recipe.
- **The same brain at the terminal** — the CLI shipped in the same install (`drift`) does everything the app does, so servers, CI pipelines and SSH sessions get the same agent as your laptop.

---

## 🧠 Simulators, First-Class

Drift is built to reach across the simulators you already use, and to speak each one on its own terms:

- **MuJoCo** — fast, contact-rich physics for humanoids, arms and quadrupeds. Drift authors MJCF scenes end-to-end, wires actuators, and runs training-friendly rollouts.
- **Gazebo** — the ROS-native workhorse. Full SDF world composition, ROS 2 bridges, sensor plugins and launch-file generation, without leaving the app.
- **NVIDIA Isaac Sim** — production-grade photorealism, USD scenes, GPU physics. Drift assembles USD stages, drives Isaac's Python API, and hands the viewport back to you.

Switching simulators is a change of intent, not a change of tools. The same natural-language plan targets any of them.

---

## 💡 What You Can Do In an Afternoon

- Spin up a humanoid in a warehouse scene and record IK-driven pick-and-place.
- Generate a Gazebo world with a moving conveyor, drop three depth cameras, and log point clouds.
- Import a URDF, ask for a MuJoCo variant with contact-rich hands, and compare stability.
- Run a controller sweep across seeds and get an inline chart, without leaving the app.
- Hand a teammate a `.drift` bundle that reproduces your whole setup, byte-for-byte.

---

## 🖥️ System Requirements

- **OS:** Ubuntu 22.04+ (or any Debian 12+ derivative)
- **Architecture:** x86_64 (arm64 coming)
- **Recommended:** a discrete GPU for Isaac Sim workflows

For simulator-specific setup (ROS 2 for Gazebo, Isaac Sim install, GPU drivers), see [the docs](https://docs.godrift.ai).

---

## 📚 Getting Started

### 1. Install

```bash
curl -fsSL https://godrift.ai/install | bash
```

### 2. Open the app

The installer launches Drift Desktop when it finishes. On a headless machine, or to open it later:

```bash
drift-desktop
```

### 3. Or use the CLI

Everything the app does is also available at the terminal:

```bash
drift
```

### 4. Ask it something real

Try any of these in the composer:

```
> author a MuJoCo scene: humanoid at spawn, kitchen counter, a mug on the counter
> import my URDF at ./arm.urdf and give me an Isaac Sim variant
> in Gazebo, build a warehouse with two AMRs and a moving conveyor
> add a lidar to my robot, rebuild, and record 10 seconds of scans
> why is the left gripper slipping on the mug?
```

---

## 🔄 Updates

Drift Desktop checks for new releases on its own and offers to install them. You never have to hunt for a version.

If you'd rather update by hand, re-running the install command is always safe — it fetches the latest signed release and takes over cleanly:

```bash
curl -fsSL https://godrift.ai/install | bash
```

---

## 🛠️ Manual Install

If you'd rather not pipe curl to bash:

1. Download the latest `.deb` from [Releases](https://github.com/godrift-ai/drift-releases/releases/latest).
2. Install:
   ```bash
   sudo dpkg -i drift_*_amd64.deb
   sudo apt-get install -f -y   # if any GTK / WebKit dependencies were missing
   ```
3. Launch:
   ```bash
   drift-desktop   # the app
   drift           # the CLI
   ```

Every release is signed. Your installed app verifies the signature of any update before it installs it — an unsigned or tampered artifact is refused.

---

## 🐛 Troubleshooting

**"Command not found: drift" after installing**
Open a new terminal (or run `hash -r`) so the shell picks up the newly installed binary.

**The app won't launch on a headless / SSH box**
Drift Desktop needs a display server (X11 or Wayland). Use the CLI (`drift`) instead — it's the same agent without the viewport.

**Dependencies missing on install**
```bash
sudo apt-get install -f -y
```

**Update seems stuck**
Re-running the install command (`curl -fsSL https://godrift.ai/install | bash`) fetches the latest and reinstalls in place.

---

## 💬 Support

- **Bugs / feature requests:** [github.com/godrift-ai/drift-releases/issues](https://github.com/godrift-ai/drift-releases/issues)
- **Docs:** [docs.godrift.ai](https://docs.godrift.ai)
- **Email:** founders@godrift.ai
- **Website:** [godrift.ai](https://godrift.ai)

---

## ❤️ Why We Built This

Robotics simulation is powerful and, today, unnecessarily hard. Half a day disappears into launch files, another half chasing a plugin version, and by the time the scene runs, the idea you started with has gone cold.

Drift Desktop is our answer: **one place that speaks Gazebo, MuJoCo and Isaac Sim, listens in English, and remembers what worked**. Students get to the interesting parts sooner. Researchers iterate without re-learning the tooling each time. Engineers ship.

Whether you're:

- 🎓 A student meeting ROS 2 for the first time
- 🔬 A researcher iterating on a novel controller
- 🏭 An engineer building a production stack
- 🤖 A hobbyist bringing your robot dream to life

**Drift Desktop is here so you can spend the day on the robot, not the tooling.**

---

## 🙏 Acknowledgments

Built on the shoulders of the open-source robotics community. Special thanks to the teams behind **Gazebo**, **MuJoCo**, **NVIDIA Isaac Sim** and **ROS 2** — and to every roboticist who has ever fought a launch file and lived to tell the tale.

---

<div align="center">

**[Get Started](https://docs.godrift.ai)** • **[View Releases](https://github.com/godrift-ai/drift-releases/releases)** • **[Get Support](https://github.com/godrift-ai/drift-releases/issues)**

Made with ❤️ by the Drift team

</div>
