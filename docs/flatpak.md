# Flatpak

## Installation and Setup

* `sudo apt install flatpak`: Install Flatpak (on Ubuntu/Debian)
* `flatpak remote-add --if-not-exists flathub https://flathub.org/repo/flathub.flatpakrepo`: Add the Flathub repository

## Managing Applications

* `flatpak install <app_id>`: Install an application
* `flatpak uninstall <app_id>`: Uninstall an application
* `flatpak update`: Update all installed applications
* `flatpak update <app_id>`: Update a specific application
* `flatpak run <app_id>`: Run an application
* `flatpak list`: List installed applications
* `flatpak search <query>`: Search for applications

## Managing Repositories

* `flatpak remote-add <name> <url>`: Add a remote repository
* `flatpak remote-delete <name>`: Remove a remote repository
* `flatpak remote-list`: List configured remote repositories
* `flatpak remote-ls <name>`: List applications available in a repository

## System Integration

* `flatpak --user override --filesystem=<path>`: Grant an app access to a specific directory
* `flatpak override --reset <app_id>`: Reset app permissions to default

## Information and Troubleshooting

* `flatpak info <app_id>`: Show detailed information about an installed application
* `flatpak history`: Show installation history
* `flatpak repair`: Repair Flatpak installation
* `flatpak document-export <file>`: Share a file with Flatpak apps

## Advanced Usage

* `flatpak build-init <directory> <app_id> <sdk> <runtime>`: Initialize a new Flatpak application
* `flatpak build <directory> <command>`: Run a command in the build environment
* `flatpak build-finish <directory> [options]`: Finish a build
* `flatpak build-export <repo> <directory>`: Export a built application to a repository

## Flatpak Permissions

* `flatpak override --show <app_id>`: Show current permissions for an app
* `flatpak override --socket=x11 <app_id>`: Grant X11 socket access to an app
* `flatpak override --nosocket=wayland <app_id>`: Revoke Wayland socket access from an app

Remember to replace `<app_id>`, `<name>`, `<url>`, `<query>`, `<path>`, `<file>`, `<directory>`, `<sdk>`, `<runtime>`, and `<repo>` with actual values when using these commands.