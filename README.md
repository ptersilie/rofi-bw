# rofi-bw

An interface to the Bitwarden CLI that uses rofi to display passwords and copy
them to the clipboard.

Requires the Bitwarden CLI (`bw`) to be installed and setup. After selecting a
password, it is immediately typed out using `xdotool`. Alternatively, the
script can be changed to copy the password to the clipboard instead (requires
uncommenting code in `rofi-bw`).

After unlocking the vault the session key is stored using Linux key management
facility `keyctl` and is purged after 1 hour, locking the vault.

## Requirements

- keyctl
- bw
- xdotool

## Installation and Usage

Download the script `rofi-bw` or clone this repository and run `./rofi-bw`. To
sync the vault press `Alt+K`.

## Configuration

- `TIMEOUT`: Time in seconds after which the Bitwarden vault is locked. Default: 3600.
- `TCLEAR`: Time in seconds after which the clipboard is cleared. Default: 10.
