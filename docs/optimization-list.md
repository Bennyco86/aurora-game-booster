# Aurora Optimization List

Aurora separates automatic, optional, and manual actions. Preview the exact current
and target values in the app before applying changes.

## Automatic Windows settings

- Enable Windows Game Mode values used by the current Windows user.
- Disable Game DVR/capture values used by the current Windows user.
- Reduce selected transparency, visual effects, and taskbar animation settings.
- Create a registry backup before supported optimizer writes.
- Verify current values after apply.

## Runtime actions

- Display top RAM processes.
- Manually trim safe process working sets above the configured threshold.
- Request a standby-list purge when Windows permits it.
- Optionally prioritize configured running game processes to `AboveNormal` while
  Aurora is running.

RAM cleanup does not add physical memory and can remove useful cache.

## Manual Windows guidance

- Open Windows gaming and graphics settings for controls that remain manual.
- Show current GPU/driver information and open official vendor update tools/pages.

## NVIDIA

Aurora previews recommended global values for power management, refresh rate,
latency, texture filtering, V-Sync, threaded optimization, shader cache, CUDA GPUs,
and OpenGL GPU selection. The planned Advanced Store candidate can apply the
supported subset through a pinned NVIDIA Profile Inspector build after the user
approves an action-specific Windows UAC prompt. Controls that cannot be verified
remain clearly marked as manual.

The Standard Store fallback does not bundle or automate NVIDIA Profile Inspector;
it keeps the complete NVIDIA checklist and opens NVIDIA's official software.

## AMD

AMD Adrenalin recommendations remain manual because controls vary by GPU and driver
version. Aurora does not write undocumented AMD driver registry values.

## Advanced Store candidate

These actions are included in the Advanced candidate and run only after an
action-specific Windows UAC confirmation:

- Enable Hardware-accelerated GPU scheduling (HAGS), with restart guidance.
- Create and activate the Ultimate Performance power plan.
- Import Aurora's supported NVIDIA global-settings subset through the pinned
  NVIDIA Profile Inspector dependency.

Microsoft must approve the restricted `allowElevation` capability before this
variant can be distributed through Microsoft Store.

## Standard Store fallback

If Microsoft does not approve the restricted capability, the Standard package
keeps the scan, backup, user-level optimizations, verification, undo, RAM/process
tools, GPU status, driver links, and manual NVIDIA/AMD guidance. It excludes HAGS,
Ultimate Performance, and NVIDIA Profile Inspector automation.

## Not included in either Microsoft Store package

- Disabling Core Isolation/Memory Integrity.
- Drive cleanup, defragmentation, or storage management.
- Automatic driver downloads or installation.
- BIOS changes.
- Instructions to bypass Windows security controls.
- Guaranteed FPS or latency claims.

The Memory Integrity implementation remains physically separate in the direct
edition for possible later distribution through a different platform. It cannot be
enabled in either Store package by changing a configuration value.
