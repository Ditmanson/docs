---
title: "Hugo installation"
date: 2026-01-16T15:26:15Z
lastmod: 2026-01-16T15:26:15Z
publishdate: 2026-01-16T15:26:15Z
draft: false
weight: 1
description: Description not needed
---
# Package manager install for you non linux people
## windows
- windows button and open cmd terminal
  - `@"%SystemRoot%\System32\WindowsPowerShell\v1.0\powershell.exe" -NoProfile -InputFormat None -ExecutionPolicy Bypass -Command "[System.Net.ServicePointManager]::SecurityProtocol = 3072; iex ((New-Object System.Net.WebClient).DownloadString('https://community.chocolatey.org/install.ps1'))" && SET "PATH=%PATH%;%ALLUSERSPROFILE%\chocolatey\bin"`
- or with powershell
  - `Set-ExecutionPolicy Bypass -Scope Process -Force; [System.Net.ServicePointManager]::SecurityProtocol = [System.Net.ServicePointManager]::SecurityProtocol -bor 3072; iex ((New-Object System.Net.WebClient).DownloadString('https://community.chocolatey.org/install.ps1'))`
### Real Windows instructions
- Pick a linux distro, i like omarchy, and dual boot your os, or better just overwrite the full partition.

## Mac
test
- open up the terminal
  - `/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"`
### Real Mac instructions
- Install ashi linux,`curl https://alx.sh | sh`
test


# [Install hugo](./installation)
- [brew install hugo](https://brew.sh/) # mac
- sudo pacman -S hugo # arch
- sudo apt install hugo # ubuntu
- sudo apt-get install hugo # debian
- sudo dnf install hugo # fedora
- [choco install hugo-extended](https://chocolatey.org/install) # windows


# [Install git](https://git-scm.com/install/)
## Windows
- [Click here to download from here. follow instructions.](https://git-scm.com/install/windows)
- [Or here is probably better because you get a bash terminal too](https://gitforwindows.org/)

## Mac
- `brew install git`

## linux
- any package manager can install git.
