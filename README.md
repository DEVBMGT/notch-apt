# Notch APT feed

This public repository contains signed Ubuntu packages for the private
[DEVBMGT/Notch](https://github.com/DEVBMGT/Notch) project.

Install the bootstrap package from a Notch release, then use Ubuntu's normal
package tools:

```bash
sudo apt install ./notch-archive-keyring_1.0.0_all.deb
sudo apt update
sudo apt install notch
```

The archive signs `dists/noble/InRelease` with this dedicated key:

`1585 5D2A 4AD1 91C9 040F 00E5 DF04 B673 C66A D977`

The feed currently targets Ubuntu Noble amd64. The keyring package installs a
`Signed-By` source configuration; no `apt-key` or privileged Notch updater is
used.
