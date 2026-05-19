# Pratfall Modding Guide

A hub for Pratfall modding!

Here you can find:
- Modding documentation
- Example mods
- Modding resources and tools

If you are working on a mod and want it listed here, feel free to reach out on our Discord server.

[![Join our Discord](https://img.shields.io/badge/Discord-Join%20Server-5865F2?logo=discord&logoColor=white)](https://discord.gg/b9EvyJKd97)

---

# Getting Started

To start creating mods for Pratfall, check out the official example mod repository:

👉 https://github.com/quad-head/pratfall-example-mod

The repository includes:
- Mod folder structure
- `manifest.json`
- `.pck` export setup
- C# code
- Example project setup

---

# Mod Structure

Mods are loaded from:

GameFolder/mods/<modname>

# Uploading Mods to Steam Workshop

Pratfall includes a `SteamWorkshopUploader.exe` tool located in the game's `mods` folder.

To upload a mod:
1. Run `SteamWorkshopUploader.exe`
2. A command line window will open
3. The tool will automatically detect available mods
4. Select the mod you want to upload
5. Follow the instructions shown in the console

The tool will then create or update the Steam Workshop item for your mod.
