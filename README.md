Here's a sample README for your GitHub repository that contains the provided Bash script:

---

# UPD - Simple Update Script for Arch Linux

This repository contains a simple Bash script to automate system maintenance tasks on a Linux machine. The script performs the following actions:

- Cleans up unnecessary files from specific directories.
- Updates system packages using `pacman` and AUR packages using `yay`.
- Prompts the user to choose whether to reboot, power off, or exit after the updates are complete.

## Script Overview

The script is divided into two main sections:

### 1. Cleanup

- **Caches**: Deletes the contents of the `~/.cache` directory.
- **Trash**: Empties the `~/.local/share/Trash` directory.

### 2. System Update

- **System Packages**: Updates all installed system packages using `pacman -Syu`.
- **AUR Packages**: Updates all installed AUR packages using `yay -Syu`.

### 3. User Prompt

After completing the updates, the script prompts the user to choose from the following actions:

1. **Reboot** (default option if no choice is made)
2. **Poweroff**
3. **Do nothing** (exit the script without further action)

## How to Use

1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/your-repo-name.git
   ```
2. Make the script executable:
   ```bash
   chmod +x maintenance.sh
   ```
3. Run the script:
   ```bash
   ./maintenance.sh
   ```

## Requirements

- **Pacman**: The script is designed for Arch Linux and its derivatives, using `pacman` as the package manager.
- **Yay**: Required for updating AUR packages. Ensure that `yay` is installed before running the script.

## Disclaimer

This script deletes files and directories. Make sure to review the code and adjust the paths according to your system configuration. Use at your own risk.

## Contributing

Feel free to fork this repository and submit pull requests to improve the script or add new features.

---

You can customize the repository name, username, or any other details as needed.
