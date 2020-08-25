# rofi-bw

An interface to the Bitwarden CLI that uses rofi to display passwords and copy
them to the clipboard.

Requires the Bitwarden CLI (`bw`) to be installed. Passwords copied to the
clipboard are automatically cleared after 10 seconds. The Bitwarden session is
stored using the Linux key management facility (`keyctl`) which will be cleared
after a specified timeout.

## Installation and Usage

Download the script `rofi-bw` or clone this repository and run `./rofi-bw`.

## Configuration

`TIMEOUT`: Time in seconds after which the Bitwarden Vault is locked. Default: 1h.
