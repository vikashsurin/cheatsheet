# DNF (Dandified YUM)

## Basic Package Management

* `sudo dnf install <package>`: Install a package
* `sudo dnf remove <package>`: Remove a package
* `sudo dnf update`: Update all packages
* `sudo dnf update <package>`: Update a specific package
* `sudo dnf check-update`: Check for available updates
* `sudo dnf clean all`: Clean all caches

## Searching and Information

* `dnf search <keyword>`: Search for packages
* `dnf info <package>`: Display information about a package
* `dnf list installed`: List all installed packages
* `dnf list available`: List all available packages
* `dnf provides <file>`: Find which package provides a specific file

## Repository Management

* `sudo dnf repolist`: List enabled repositories
* `sudo dnf repolist all`: List all repositories (enabled and disabled)
* `sudo dnf config-manager --add-repo <repo_url>`: Add a new repository
* `sudo dnf config-manager --set-enabled <repo>`: Enable a repository
* `sudo dnf config-manager --set-disabled <repo>`: Disable a repository

## Group Management

* `sudo dnf group list`: List available groups
* `sudo dnf group install <group_name>`: Install a group of packages
* `sudo dnf group remove <group_name>`: Remove a group of packages

## History and Rollback

* `sudo dnf history`: View DNF transaction history
* `sudo dnf history info <id>`: View detailed information about a specific transaction
* `sudo dnf history undo <id>`: Undo a specific transaction
* `sudo dnf history rollback <id>`: Rollback to a specific transaction

## Plugins and Modules

* `dnf plugin list`: List available plugins
* `sudo dnf install dnf-plugins-core`: Install core DNF plugins
* `dnf module list`: List available modules
* `sudo dnf module install <module>`: Install a specific module
* `sudo dnf module enable <module>`: Enable a specific module

## System Upgrade

* `sudo dnf upgrade`: Upgrade packages (same as update)
* `sudo dnf system-upgrade download --releasever=<version>`: Download packages for system upgrade
* `sudo dnf system-upgrade reboot`: Reboot and perform system upgrade

## Advanced Usage

* `sudo dnf reinstall <package>`: Reinstall a package
* `sudo dnf downgrade <package>`: Downgrade a package
* `sudo dnf autoremove`: Remove unnecessary packages
* `sudo dnf mark install <package>`: Mark a package as user-installed
* `sudo dnf mark remove <package>`: Mark a package as automatically-installed
* `dnf repoquery <package>`: Query the package database

## Configuration

* `sudo dnf config-manager --setopt=<option>=<value>`: Set a DNF configuration option
* `dnf config-manager --dump`: Display current DNF configuration

Remember to replace `<package>`, `<keyword>`, `<file>`, `<repo_url>`, `<repo>`, `<group_name>`, `<id>`, `<module>`, `<version>`, and `<option>` with actual values when using these commands.