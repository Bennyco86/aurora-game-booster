# Aurora Game Booster Support

Updated: 2026-07-29

Email: `nzbennycohen@gmail.com`

## Blocked by Smart App Control

Do not turn off Smart App Control to run Aurora. Delete or quarantine the downloaded
installer and send the following information to the support email:

```powershell
Get-FileHash "$env:USERPROFILE\Downloads\AuroraGameBoosterSetup-1.0.17.exe" -Algorithm SHA256
Get-AuthenticodeSignature "$env:USERPROFILE\Downloads\AuroraGameBoosterSetup-1.0.17.exe" |
    Select-Object Status, StatusMessage
```

For the original Aurora `1.0.17` build, the expected SHA-256 was:

```text
F55A9C3BDA3CA5E263884DBB493E4B6A02F4044BB25569379B41583434A26F58
```

A matching checksum only confirms the file matches the original release; it does not
instruct Windows to trust or run it. Microsoft's case is completed and its latest
verified cloud and client results showed `No malware detected`, but the portal's
final-determination column still showed `Pending`. Distribution remains paused until
the case is rechecked and the exact installer passes a current Smart App Control
retest.

Microsoft case:
<https://www.microsoft.com/en-us/wdsi/submission/ebef05f6-3719-49ee-8ecb-4639f3c42fcf>

## Private beta support

Contact the person who provided the beta installer. Include the information below,
but remove personal details from screenshots and logs first.

```text
Aurora version:
Windows version:
CPU:
GPU and driver version:
Installed RAM:
Ran as Administrator: Yes / No

Action performed:
Expected result:
Actual result:
Exact error text:
Restart completed: Yes / No
Undo attempted: Yes / No
```

Attach only the relevant Aurora log lines. Do not send complete registry backups,
license keys, passwords, or unrelated system logs.

## Before reporting a problem

1. Confirm the Aurora version shown in the installer or release notes.
2. Restart Windows if the app says a restart is required.
3. Run Preview Planned Changes again and note the current and target values.
4. Check whether the action is labelled automatic, manual, or experimental.
5. Record the exact timestamp and corresponding log lines.
