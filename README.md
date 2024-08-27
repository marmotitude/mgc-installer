# MGC CLI Installer Script

This repository contains a Bash script for installing the MGC CLI tool from MagaluCloud. The script automates the process of downloading, verifying, and installing the MGC CLI on supported Unix-based operating systems.

## Supported Operating Systems

- Linux
- FreeBSD
- NetBSD
- OpenBSD
- macOS

## Prerequisites

Before running the script, ensure that you have the following tools installed:

- `tar` (for extracting the downloaded archive)
- `curl` or `wget` (for downloading the necessary files)

## Installation

To install the MGC CLI using this script, run the following command:

```bash
sudo -v ; curl https://mgc-cli.br-se1.magaluobjects.com/install.sh | sudo bash
```

Tool Verification: The script checks for the presence of supported tools (tar) to extract the downloaded archive.

Download the Latest Version: The script fetches the latest version of MGC CLI from the GitHub releases page.

Platform Detection: The script determines the operating system and architecture to download the correct binary.

Install MGC CLI: The binary is copied to the appropriate location (/usr/bin/mgc for Linux and similar systems).

Cleanup: Temporary files are deleted after installation.

Post-Installation: The script confirms the installation and provides a link to the configuration guide.

Uninstallation
To remove the MGC CLI, simply delete the installed binary:

```bash
sudo rm /usr/bin/mgc
```

Troubleshooting
If you encounter any issues during the installation, ensure that:

You are running a supported operating system.
The required tools (tar, curl, wget) are installed and available in your system's PATH.
For further help, visit the MGC CLI documentation.

License
This script is provided under the MIT License. See the LICENSE file for more details.
