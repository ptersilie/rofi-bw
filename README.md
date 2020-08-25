# rofi-bw

An interface to the Bitwarden CLI that uses rofi to display passwords and copy
them to the clipboard.

Requires the Bitwarden CLI (`bw`) to be installed and setup. By default,
passwords copied to the clipboard are automatically cleared after 10 seconds,
and the Bitwarden session (which is stored stored using the Linux key
management facility `keyctl`), is purged after 1 hour, locking the vault.

## Installation and Usage

Download the script `rofi-bw` or clone this repository and run `./rofi-bw`.

## Configuration

`TIMEOUT`: Time in seconds after which the Bitwarden vault is locked. Default: 3600.
`TCLEAR`: Time in seconds after which the clipboard is cleared. Default: 10.
