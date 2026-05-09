
# 🍓 Raspberry Pi 4 - Complete Setup & Command Guide

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Raspberry Pi](https://img.shields.io/badge/Raspberry%20Pi-4-blue)](https://www.raspberrypi.com/products/raspberry-pi-4-model-b/)

A comprehensive guide for setting up, configuring, and managing your **Raspberry Pi 4** - from beginner basics to advanced networking commands.

## 📋 Table of Contents
- [About this Repository](#about-this-repository)
- [Raspberry Pi 4 Overview](#raspberry-pi-4-overview)
- [Operating Systems](#operating-systems)
- [Quick Start](#quick-start)
- [Essential Commands](#essential-commands)
- [SSH & Network Setup](#ssh--network-setup)
- [Repository Structure](#repository-structure)
- [Contributing](#contributing)

## 🎯 About this Repository

This repository is your one-stop resource for:
- **Understanding Pi 4 hardware capabilities**
- **Installing and comparing OS options** (Raspberry Pi OS, Ubuntu 22.04)
- **Mastering essential terminal commands**
- **Connecting via SSH** (Ethernet & Wi-Fi)
- **Network troubleshooting** commands that actually work

> ⚠️ **Note:** This guide is specifically for **Raspberry Pi 4 Model B**. Some commands/configurations may differ on Pi 3, Pi 5, or Zero models.

## 🖥️ Raspberry Pi 4 Overview

| Specification | Details |
|--------------|---------|
| **CPU** | Broadcom BCM2711, Quad-core Cortex-A72 @ 1.5GHz |
| **RAM** | 2GB / 4GB / 8GB LPDDR4 |
| **Wi-Fi** | 802.11ac Dual-band (2.4GHz & 5GHz) |
| **Bluetooth** | Bluetooth 5.0 (BLE) |
| **Ethernet** | Gigabit Ethernet |
| **USB Ports** | 2× USB 3.0 + 2× USB 2.0 |
| **Video** | 2× Micro HDMI (up to 4Kp60) |
| **Power** | USB-C (5V/3A recommended) |
| **GPIO** | 40-pin header |
| **Storage** | MicroSD card (USB boot also available) |

### When to use Pi 4?
✅ **Great for:** Desktop replacement, media center (4K), home server, robotics, IoT hub, lightweight web server  
❌ **Not ideal for:** Heavy video editing, AAA gaming, machine learning training

## 💿 Operating Systems

### [Raspberry Pi OS](operating-systems/raspberry-pi-os.md)
- **Based on:** Debian
- **Optimized for:** Pi hardware (GPU, GPIO, camera)
- **Versions:** 32-bit & 64-bit (recommend 64-bit for Pi 4)
- **Best for:** Beginners, GPIO projects, educational use
- **Key tool:** `raspi-config`

### [Ubuntu 22.04 LTS](operating-systems/ubuntu-22-04.md)
- **Based on:** Ubuntu Jammy Jellyfish
- **Optimized for:** Server workloads, multi-user environments
- **Versions:** Desktop, Server (minimal)
- **Best for:** Docker/K8s, web servers, ROS, development
- **Note:** Some Pi-specific tools need manual setup

## 🚀 Quick Start

### Minimal setup (3 steps):
1. **Download** Raspberry Pi Imager from [raspberrypi.com/software](https://www.raspberrypi.com/software/)
2. **Flash** your chosen OS to a microSD card (16GB+ recommended)
3. **Enable SSH** (see [SSH Setup](#ssh--network-setup))

```bash
# First boot - default credentials
Username: pi
Password: raspberry

# Immediately change password!
passwd
