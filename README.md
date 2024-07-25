# dwmexit-demu
This script is designed for Arch Linux systems running the dwm window manager + dmenu and using systemd for service management. It integrates with dmenu to provide a convenient way to handle common system actions directly from your dwm environment.

## Features

- Suspend: Puts the system into sleep mode. A notification is displayed for 3 seconds before the system is suspended.
- Kill DWM: Terminates the dwm window manager. You are prompted to confirm this action. A notification is shown for 3 seconds before dwm is killed.
- Log Out: Logs you out of your current session. Confirmation is required, and a notification is shown for 3 seconds before logging out.
- Reboot: Reboots the system. You will be asked to confirm this action, and a notification is displayed for 3 seconds before the system reboots.
- Shutdown: Powers off the system. Confirmation is required, and a notification is shown for 3 seconds before shutting down the system.
- Exit Script: Closes the script without performing any actions.

# Usage

- Placement: Save this script as /usr/local/bin/dwmexit-dmenu. This location is suitable for user-defined scripts and ensures that the script is accessible from anywhere in your system.
- Permissions: After saving the script, you need to make it executable. Run the following command to set the appropriate permissions: sudo chmod +x /usr/local/bin/dwmexit-dmenu
- Run this script from dmenu by executing dwmexit-dmenu. The script will display a menu with the above options.
Select the desired action using dmenu, and follow the prompts for confirmation where applicable.

# Requirements

- dmenu: A dynamic menu for X.
- notify-send: A command-line tool for sending desktop notifications.
