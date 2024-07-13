# <!-- Home -->

[![DockSTARTer](https://github.com/GhostWriters/DockSTARTer/raw/master/docs/assets/logo.png)](https://dockstarter.com)

[![Supporters on Open Collective](https://img.shields.io/opencollective/all/DockSTARTer.svg?style=flat-square&color=607D8B&logo=opencollective&logoColor=white)](#supporters)
[![Discord chat](https://img.shields.io/discord/477959324183035936.svg?style=flat-square&color=607D8B&logo=discord&logoColor=white)](https://dockstarter.com/discord)
[![GitHub contributors](https://img.shields.io/github/contributors/GhostWriters/DockSTARTer.svg?style=flat-square&color=607D8B&logo=github&logoColor=white)](https://github.com/GhostWriters/DockSTARTer/graphs/contributors)
[![GitHub last commit master](https://img.shields.io/github/last-commit/GhostWriters/DockSTARTer/master.svg?style=flat-square&color=607D8B&logo=github&logoColor=white&label=code%20committed)](https://github.com/GhostWriters/DockSTARTer/commits/master)
[![GitHub license](https://img.shields.io/github/license/GhostWriters/DockSTARTer.svg?style=flat-square&color=607D8B&logo=github&logoColor=white)](https://github.com/GhostWriters/DockSTARTer/blob/master/LICENSE.md)
[![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/GhostWriters/DockSTARTer/tests.yml?style=flat-square&color=607D8B&logo=github&logoColor=white&branch=master)](https://github.com/GhostWriters/DockSTARTer/actions?query=workflow%3ARun%20Tests+branch%3Amaster)

The main goal of DockSTARTer is to make it quick and easy to get up and running with Docker.

You may choose to rely on DockSTARTer for various changes to your Docker system or use DockSTARTer as a stepping stone and learn to do more advanced configurations.

![Main Menu](https://i.imgur.com/odfRk0j.png)

![App Select](https://i.imgur.com/tFsu2Hh.png)

![Value Prompt](https://i.imgur.com/k1bdAoQ.png)

![Command Line Interface](https://i.imgur.com/Y8F3uT2.png)

## Getting Started

### System Requirements

- You must be running a [supported platform](https://docs.docker.com/install/#supported-platforms) or an operating system based on a supported platform. Platforms named below will link to documentation listing compatible versions.
- You must be logged in as a non-root user with sudo permissions.

### One Time Setup (required)

- APK Systems (Alpine)

  ```bash
  sudo apk add curl git
  bash -c "$(curl -fsSL https://mnlx.link/DockSTARTer)"
  sudo reboot
  ```

- APT Systems ([Debian](https://docs.docker.com/install/linux/docker-ce/debian/#os-requirements), [Ubuntu](https://docs.docker.com/install/linux/docker-ce/ubuntu/#os-requirements), etc)

  ```bash
  sudo apt-get install curl git
  bash -c "$(curl -fsSL https://mnlx.link/DockSTARTer)"
  sudo reboot
  ```

  > Raspbian requires a few extra commands

  ```bash
  sudo apt-get update
  sudo apt-get dist-upgrade
  sudo apt-get install curl git
  bash -c "$(curl -fsSL https://get.docker.com)"
  bash -c "$(curl -fsSL https://mnlx.link/DockSTARTer)"
  sudo reboot
  ```

  > OpenMediaVault (OMV) requires [special instructions found here](https://dockstarter.com/advanced/openmediavault/)

- DNF Systems ([Fedora](https://docs.docker.com/install/linux/docker-ce/fedora/#os-requirements))

  ```bash
  sudo dnf install curl git
  bash -c "$(curl -fsSL https://mnlx.link/DockSTARTer)"
  sudo reboot
  ```

- Pacman Systems (Arch, Manjaro, EndeavourOS, etc.)

  ```bash
  sudo pacman -Sy curl docker git
  bash -c "$(curl -fsSL https://mnlx.link/DockSTARTer)"
  sudo reboot
  ```

- YUM Systems ([CentOS](https://docs.docker.com/install/linux/docker-ce/centos/#os-requirements))

  ```bash
  sudo yum install curl git
  bash -c "$(curl -fsSL https://mnlx.link/DockSTARTer)"
  sudo reboot
  ```

<details>
  <summary>Alternate install (any system)</summary>

The standard install above downloads the initial script using a method with some known risks. For those concerned with the security of the above method, here is an alternative:

```bash
## NOTE: Run the appropriate command for your distro
sudo apt-get install curl git
sudo dnf install curl git
sudo pacman -Sy curl git
sudo yum install curl git
```

Then

```bash
git clone https://github.com/s3tupw1zard/DockSTARTer "/home/${USER}/.docker"
bash /home/"${USER}"/.docker/main.sh -vi
sudo reboot
```

</details>

### Running DockSTARTer

```bash
ds
```

To run DockSTARTer, use the command above. You should now see the main menu from the screenshots. Select `Configuration` and then `Full Setup`, and you will be guided through selecting apps and starting containers.

See our [documentation](https://dockstarter.com/introduction/) for more detailed information.

## NOTE

This is just for me personally. Please use the original project at [GhostWriters/DockSTARTer](https://github.com/GhostWriters/DockSTARTer)