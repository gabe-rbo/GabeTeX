# Changelog

This is the overview changelog of the GabeTeX umbrella repository. Each app keeps its own detailed changelog and
release notes:

| Platform | Changelog | Releases |
|---|---|---|
| macOS | [GabeTeX-macOS/CHANGELOG.md](https://github.com/gabe-rbo/GabeTeX-macOS/blob/main/CHANGELOG.md) | [Releases](https://github.com/gabe-rbo/GabeTeX-macOS/releases) |
| Linux | [GabeTeX-Linux/CHANGELOG.md](https://github.com/gabe-rbo/GabeTeX-Linux/blob/main/CHANGELOG.md) | In development |
| Windows | [GabeTeX-Windows/CHANGELOG.md](https://github.com/gabe-rbo/GabeTeX-Windows/blob/main/CHANGELOG.md) | In development |

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/).

## [Unreleased]

### Changed

- The repository is now an umbrella with three Git submodules: `GabeTeX-macOS`, `GabeTeX-Linux` and
  `GabeTeX-Windows`. Application code, builds, releases and platform-specific issues live in those repositories.
- The website (`docs/`) stays here; its download and release links point to GabeTeX-macOS.

## Overview of releases

- **macOS 1.0.0** (2026-10-29): first public release of GabeTeX for macOS. See the
  [macOS changelog](https://github.com/gabe-rbo/GabeTeX-macOS/blob/main/CHANGELOG.md).
- **Linux, Windows**: in development (Tauri 2), no releases yet.
