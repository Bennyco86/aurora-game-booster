# Aurora Game Booster Beta Notice

Updated: 2026-07-29

Aurora Game Booster is prerelease software. It changes supported Windows gaming
settings only after showing the planned changes, but results and compatibility vary
by PC, Windows version, drivers, security configuration, and game.

## Smart App Control

Do not disable Smart App Control or other Windows security features just to install
Aurora. If Windows blocks the installer, stop and report the Aurora version, download
source, SHA-256 checksum, and a screenshot to `nzbennycohen@gmail.com`.

Aurora `1.0.17` remains on distribution hold after a beta tester received a Smart
App Control malware warning. Microsoft completed submission
`ebef05f6-3719-49ee-8ecb-4639f3c42fcf`; the latest verified cloud and client results
showed `No malware detected`, and the analyst comment was favorable. However, the
portal's final-determination column still showed `Pending` on `2026-07-27`.

Do not redistribute the build until the case is rechecked and the exact installer
passes a current Smart App Control retest. Do not disable Windows security controls
to perform that test.

## Before testing

1. Create a Windows restore point.
2. Close games and save important work.
3. Review Preview Planned Changes before applying anything.
4. Create an Aurora backup and confirm that the backup is listed.
5. Leave aggressive or experimental options off unless you understand the tradeoff.

## Important limitations

- Aurora does not guarantee an FPS increase.
- Clearing RAM does not add physical memory and can temporarily remove useful cache.
- Disabling Memory Integrity reduces Windows security and requires explicit consent.
- HAGS and some driver settings can help, hurt, or make no measurable difference
  depending on the hardware and game.
- Registry backup is useful for Aurora-managed changes but is not a replacement for
  a full Windows restore point or system backup.
- NVIDIA automation is experimental and only covers settings explicitly shown by
  the app.

If a game, device, or Windows feature behaves unexpectedly, stop applying changes,
use Aurora's undo function where available, and report the exact action and log text.
