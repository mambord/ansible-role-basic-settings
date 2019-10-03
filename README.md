# ansible-role-basic-settings

This role does some basic settings and packet installation on Debian systems.

## /etc/apt/sources.list
```
deb http://ftp.de.debian.org/debian/ stable main non-free
deb http://ftp.de.debian.org/debian/ stable-updates main non-free
deb http://security.debian.org/ stable/updates main
```

## Sysctl
```
# variable to disable IPv6. enabled by default.
basicsettings_disable_ipv6: yes
```
## Packet installation
```
# variable with list of packages to install
basicsettings_packages:
  - vim
  - curl
  - htop
  - screen
```
