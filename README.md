# 📡 UWB 3D Localization Engine (Legacy Core)

![Language](https://img.shields.io/badge/Language-C++-blue.svg) ![Hardware](https://img.shields.io/badge/Hardware-Decawave_DW1000-orange.svg) ![Status](https://img.shields.io/badge/Status-Archived-lightgrey.svg)

> **Note:** This is a foundational codebase developed in 2020, focusing on the core mathematical algorithms for 3D positioning using Ultra-Wideband (UWB) technology. For my latest work on Radar & Robotics, please visit **[Project Fire-Gecko](https://github.com/Dr-CharleyChang/Dr-CharleyChang)**.

## 📖 Overview
This repository hosts a high-performance **3D Localization & Tracking System** designed for Decawave DW1000-based hardware. It implements a complete signal processing pipeline from raw serial data to precise coordinate calculation.

Unlike modern high-level Python scripts, this project is written in **pure C++**, optimized for embedded systems and real-time processing performance.

## 🧩 Key Modules
Based on the file structure, this engine includes:

* **`ctaglocalg` (Localization Algorithm)**: Core solver for calculating (x, y, z) coordinates using TDOA/TOA trilateration.
* **`ctagtrackal` (Tracking Algorithm)**: Implements trajectory smoothing (likely Kalman Filter or similar) to reduce jitter.
* **`ccmath` & `ccsp`**: Custom Math & Signal Processing libraries optimized for embedded environments.
* **`cserialport` & `ctcpcom`**: Robust communication layer handling Serial (UART) and TCP/IP data streams.

## 🛠️ Tech Stack
* **Language**: C++ (98.8%)
* **Hardware**: Decawave DW1000 Series
* **Methods**: Least Squares Estimation, Geometric Dilution of Precision (GDOP) Optimization.

---
*Copyright © 2020-2025 Dr. Charley Chang. All Rights Reserved.*
