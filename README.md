# Provenance — versioned asset library for Blender

Provenance is a local-first, versioned asset vault for Blender. Publish any
selection as a snapshot, build up a version history over time, and bring any
earlier version back into a scene whenever you need it.

- **Publish** selected objects into a local vault folder as numbered versions
  (`v001`, `v002`, …), each tagged, timestamped and stored as its own
  standalone `.blend` file.
- **Dependency reports** before you insert: triangle count, material count,
  image count and estimated external texture size, so you know what you are
  bringing in before it is in your scene.
- **Link Surgery**: scans the open file for broken external references,
  missing textures or linked libraries and relinks them automatically when
  the right candidate is unambiguous — and refuses to guess when it is not.
- Vault files are plain `.blend` files: they open in a stock Blender without
  this add-on installed.

## Compatibility

Blender **4.2 or newer** (tested on 4.2.x and 5.2.x LTS) on Windows, macOS and
Linux. No third-party dependencies, no accounts, no network access — the vault
is a folder on your machine.

## Installation

Install `provenance_extension.zip` from the
[Blender extensions site](https://extensions.blender.org/add-ons/provenance/)
(*Edit → Preferences → Get Extensions*, or *Install from Disk*). Before your
first publish, set the vault folder in
*Edit → Preferences → Add-ons → Provenance → Vault Root*.

## Reporting issues

This repository is the **public bug tracker** for Provenance. Please open an
issue for bugs, crashes, incorrect restores or feature requests, including:

1. the Provenance version (*Preferences → Add-ons → Provenance*),
2. the Blender version and build (*Help → About Blender*),
3. your operating system,
4. step-by-step reproduction, and the vault or scene file if you can share it.

## License

GPL-3.0-or-later © 2026 Metanoid. Every source file carries a copyright and
license header, and the full license text ships inside the add-on package.
