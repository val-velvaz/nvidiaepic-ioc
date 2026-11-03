# NVIDIAEpic.py / RazerControlCenter malware: IOCs and removal guide

Indicators of compromise (IOCs) and cleanup steps for a **ClickFix** infection (fake captcha → Win+R → PowerShell) that installs:

- A Python **crypto clipper**: `C:\ProgramData\RazerControlCenter\NVIDIAEpic.py`, started from `HKCU\Software\Microsoft\Windows\CurrentVersion\Run\NVIDIAEpic`.
- A **malicious Edge extension** posing as *"Save to Google Drive"* by *"Google inc."*.
- A PowerShell loader (`%TEMP%\S422.ps1`) that runs an encrypted payload in memory, most likely an infostealer.

Full guide: `index.html` (English) · `es.html` (Español), or the published GitHub Pages site.

## Hashes (SHA-256)

| File | SHA-256 |
|---|---|
| `NVIDIAEpic.py` | `e79386ac66b0f3a07f063b444e390c50ac744597c27f968a211de4ff275f3d7b` |
| `S422.ps1` | `693e46e9bb68c0c74bf84d7ed9b3bfcc14ab0d67ae0b1be59aaabac254ac551e` |

## Network (defanged)

- `hxxp://45.155.69[.]180/yrjrs/sava.ra`
- `hya.codedevfuture[.]buzz`
- `breakthroughdev[.]buzz`

This repository **does not contain any malware samples**, only indicators and documentation.

Have more hashes, folder names or domains from this campaign? Please open an issue.