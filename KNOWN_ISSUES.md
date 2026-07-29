# Aurora Game Booster Known Issues

Updated: 2026-07-29

## Distribution status

Aurora `1.0.17` is on distribution hold. Microsoft completed the submitted Smart App
Control case and the latest verified cloud and client results showed no malware, but
the portal's final-determination column still showed `Pending`. Do not redistribute
this build until the case is rechecked and the exact installer passes a current
Smart App Control retest.

## Installer trust

The `1.0.17` installer and launcher are unsigned. Do not disable Windows security
controls to run a blocked installer. The selected public route is a new Microsoft
Store MSIX, which Microsoft signs after successful Store certification. The held
direct installer is not the Store release candidate.

## Store edition limits

The Advanced Store candidate includes HAGS, Ultimate Performance, and pinned NVIDIA
Profile Inspector automation behind action-specific UAC. It cannot be published
unless Microsoft approves the restricted `allowElevation` capability. The Standard
fallback excludes those three features.

Neither Store package contains the direct-edition Memory Integrity implementation.

## Administrator actions

The Advanced Store candidate requests Administrator access only when an advanced
action is selected. The separate direct/development edition may also require an
Administrator launch for its advanced actions.

## Restart state

HAGS requires a Windows restart whether it is applied by the Advanced Store candidate
or the direct edition. Memory Integrity remains direct-edition-only.

## RAM clearing

Clearing working sets or standby memory does not add physical RAM. It can remove
useful cache and may temporarily reduce performance. Use it only when troubleshooting
memory pressure, not as a guaranteed FPS boost.

## NVIDIA automation

NVIDIA global-profile automation is experimental. The Advanced Store candidate pins
Profile Inspector `3.0.2.1` and requests UAC for import. The Standard fallback offers
manual NVIDIA guidance only.

## AMD settings

AMD Adrenalin settings remain a manual checklist because available controls differ by
GPU, driver branch, and Adrenalin version.

## Support

Report issues to `nzbennycohen@gmail.com` with the Aurora version, Windows version,
GPU/driver, exact action, error text, and only the relevant sanitized log lines.
