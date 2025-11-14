# RumbleBumble-Scripts

Assorted hardening helpers for CyberPatriot-style practice environments.

## Linux Mint 21 hardening script

The file `linux scrpt` automates the most common steps from the slide deck on Linux Mint 21.x desktops. This is the only maintained Linux script; the old `linuxscirptTemporary` file has been removed.

### How to run

```bash
chmod +x "linux scrpt"
sudo bash "./linux scrpt"
```

**Heads-up:** the script changes your SSH port, disables root login, and turns off IPv6. Run it from a local console on a Mint machine or ensure you have alternate access before proceeding.

See `InstructionsForLinuxScript` for the same step-by-step guidance you get on Windows.

### After running

- Reconnect over SSH using the new port displayed at the end of the script.
- Review the generated backups in `/etc/*.bak.*` if you need to revert any configuration files.
- Complete the manual checklist printed by the script (user accounts, screen lock, hidden files, and ClamAV scans).

