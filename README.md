# revert_upgrade

A simple way to revert an Arch Linux upgrade that broke something.
A hook saves the versions of the upgraded packages before performing the upgrade and saves them in a file so that you can easily downgrade all upgraded packages at once later.
Depends on [expac](https://github.com/falconindy/expac).
Package lists are created in `/usr/share/upgrades/`, and files older than 14 days are deleted automatically.

## Usage

```sh
revert_upgrade /usr/share/upgrades/latest
```
