# 🛠 Project Setup Guide: Flux Defense

This document provides instructions for setting up the development environment to run and contribute to **Flux Defense**.

## 1. Prerequisites

To ensure compatibility with advanced **Type Hinting** and **Pygame-ce** features, please follow these requirements:

* **Python Version:** `3.14.2`.
* **Operating System:** Windows 10/11, macOS, or Linux.
* **Package Manager:** `pip`.

## 2. Virtual Environment Setup

Using a virtual environment is **mandatory** to avoid dependency conflicts.

### Windows:
```bash
# Create virtual environment
python -m venv venv

# Activate virtual environment
.\venv\Scripts\activate
```

## 3. Installation
Once the virtual environment is active, install the required packages:
```bash
pip install --upgrade pip
pip install pygame-ce mypy
```
Note: Use `pygame-ce` (Community Edition) for better performance and frequent updates.

## 4. Project structure
```text
flux-defense/
├── assets/             # Sprites, SFX, Fonts
├── src/                # Source code
│   ├── entities/       # Player, Turret, Enemy classes
│   ├── engine/         # Core logic, Physics, Wave Management
│   └── utils/          # Type Aliases, Constants
├── main.py             # Entry point
├── requirements.txt    # Dependency list
└── SETUP.md            # This guide
```

## 5. Running the Game
To launch the application:
```bash
python main.py
```

To run static type checking:
```bash
mypy main.py
```

## 6. Export requirments.txt after installing new package
```bash
pip freeze > requirements.txt
```