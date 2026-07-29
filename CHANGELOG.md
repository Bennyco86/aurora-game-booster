# Changelog

All notable changes to Aurora Game Booster are recorded here.

## 1.0.18 - Unreleased

### Added

- Reproducible Microsoft Store MSIX build and package-validation scripts.
- Store-specific writable logs/backups under `%LOCALAPPDATA%\AuroraGameBooster`.
- Per-monitor high-DPI launcher manifest for mixed-resolution displays.
- Standard and Advanced Store package variants.
- Action-specific elevated helper for HAGS, Ultimate Performance, and NVIDIA preset
  import in the Advanced candidate.
- Pinned NVIDIA Profile Inspector `3.0.2.1` with verified hashes and MIT notice.

### Store safety

- Main Store UI remains non-elevated; Advanced UAC is requested only when used.
- Advanced helper accepts three allow-listed operations rather than arbitrary input.
- Memory Integrity implementation moved to a direct-edition-only module and is not
  packaged in either Store variant.
- Standard fallback contains no elevated helper or NVIDIA Profile Inspector.
- Existing direct/Inno behavior remains separate.

## 1.0.17 - 2026-07-26

### Added

- Installed NVIDIA and AMD GPU model, driver version, driver date, and device-status display.
- NVIDIA release-style version conversion alongside the Windows driver version.
- `Check in NVIDIA App` and `AMD Software / Check Updates` vendor-check actions.
- Official NVIDIA and AMD driver-download buttons with vendor-app fallback behavior.

### Safety

- Aurora does not label a driver current or outdated from its date alone and does not download or install GPU drivers.

## 1.0.16 - 2026-07-26

### Added

- NVIDIA Profile Inspector auto-apply for `CUDA - GPUs = All`.
- Dynamic NVIDIA OpenGL rendering GPU detection and string-profile import.

### Changed

- Only Resizable BAR remains a manual NVIDIA item because it depends on hardware and BIOS support.

## 1.0.15 - 2026-07-26

### Changed

- Reorganized the main window around a numbered Scan, Backup, Apply, Verify workflow.
- Added workflow guidance that updates after each recommended action.
- Moved security, HAGS, power-plan, and Windows settings controls into a collapsed Advanced section.
- Grouped NVIDIA and AMD controls into a dedicated graphics-driver section.
- Made optimization plan and verification the dominant table above the smaller RAM monitor.
- Added status legends and prioritized target/details columns in the verification table.
- Collapsed the activity log by default to reduce visual clutter.

## 1.0.14 - 2026-07-26

### Added

- AMD Radeon GPU detection.
- Performance-oriented Radeon/Adrenalin recommendations in preview and apply results.
- Plain-language Radeon setting explanations and tradeoffs.
- `Open AMD Software` launcher with best-effort monitor placement.
- Private beta preparation and public documentation.

## 1.0.13 - 2026-04-06

### Added

- Setup-once optimization preview, apply-missing, verification, and undo workflow.
- Registry backup before supported Windows setting changes.
- RAM and process monitor with manual and scheduled cleanup.
- Configured game-process priority while games are running.
- Optional Ultimate Performance power-plan action.
- Optional advanced HAGS and Memory Integrity controls with restart and security warnings.
- Experimental NVIDIA Profile Inspector preset import for supported global settings.
- NVIDIA Control Panel and NVIDIA Profile Inspector download shortcuts.
- Resizable main, preview, and explanation windows.
- Aurora application and installer icon.

### Safety

- Drive cleanup is not included.
- Power plans are not changed by the normal optimizer action.
- Security-reducing changes require explicit selection.
- Manual, experimental, and verified actions are labelled separately.
