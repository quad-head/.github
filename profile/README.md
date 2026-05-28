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

# Console Logging

By default, Godot does not immediately flush normal log output (`GD.Print`) to the console. This can make debugging mods more difficult.

To enable immediate console flushing, create an `override.cfg` file next to the game executable with the following content:

```ini
[application]

run/flush_stdout_on_print=true
```

# Uploading Mods to Steam Workshop

Pratfall includes a `SteamWorkshopUploader.exe` tool located in the game's `mods` folder.

To upload a mod:
1. Run `SteamWorkshopUploader.exe`
2. A command line window will open
3. The tool will automatically detect available mods
4. Select the mod you want to upload
5. Follow the instructions shown in the console

The tool will then create or update the Steam Workshop item for your mod.

The uploader stores the Steam Workshop item ID in a `workshop_manifest.json` file inside the mod folder. This file is used to determine whether the uploader should create a new Workshop item or update an existing one.

If you delete your Workshop item through the Steam Workshop website or Steam UI, you must also delete the local `workshop_manifest.json` file before uploading again. Otherwise, the uploader will attempt to update a Workshop item that no longer exists.

# Steam Workhsop Preview Image

To upload a Steam Workshop preview image, place a `Preview.png`, `Preview.jpg`, or similar image file inside your mod folder. The uploader will automatically use this image as the Workshop thumbnail. The image size limit is 1 MB.

# Examples

Example Mod: https://github.com/quad-head/pratfall-example-mod

Infinite Flare Mod: https://github.com/quad-head/pratfall-infinite-flare-mod

# From the Community

APratfallModFramework: https://github.com/unexpear/APratfallModFramework
