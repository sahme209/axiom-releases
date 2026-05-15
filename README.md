# Axiom Agent — Desktop Releases

This repository hosts the public, downloadable binaries for the **Axiom Agent** desktop app
(https://visionxixlabs.com/download). The source code lives in a private repository; only the
release artefacts ship here so any visitor can install without authentication.

## Latest builds

Releases are tagged `desktop-v*` and built by GitHub Actions in the source repo. Each release
ships:

- `Axiom Agent_<ver>_aarch64.dmg` — macOS Apple Silicon (signed + notarized)
- `Axiom Agent_<ver>_x64.dmg` — macOS Intel (signed + notarized)
- `Axiom Agent_<ver>_x64-setup.exe` — Windows x64 installer (unsigned — see install notes)
- `Axiom Agent_<ver>_x64_en-US.msi` — Windows x64 MSI (unsigned)
- `Axiom Agent_<ver>_amd64.AppImage` — Linux universal (chmod +x to run)
- `Axiom Agent_<ver>_amd64.deb` — Debian/Ubuntu
- `Axiom Agent-<ver>-1.x86_64.rpm` — RHEL/Fedora

See the **Releases** tab for the latest version.

## Install notes

- **macOS:** Double-click the DMG → drag Axiom Agent to Applications. Signed by Vision XIX Labs LLC.
- **Windows:** Run the `.msi`. SmartScreen may show a one-time "More info → Run anyway" prompt
  until an EV cert is added.
- **Linux:** `chmod +x ./Axiom-Agent_*.AppImage` and run, or `sudo dpkg -i` / `sudo rpm -i` for
  the distro-specific packages.

## What does Axiom Agent do?

It is a local operations workstation for Axiom's autonomous cloud operations control plane.
The desktop app reads your workspace state from https://visionxixlabs.com — sign in there
first and the desktop will pick up your session.

## Reporting issues

Please file issues on the main project page at https://visionxixlabs.com.

— Vision XIX Labs LLC
