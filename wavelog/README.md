# Home Assistant Add-on: Wavelog

_Installs the latest release of wavelog from github_

[Wavelog](https://github.com/wavelog)

![Supports amd64 Architecture][amd64-shield]

[amd64-shield]: https://img.shields.io/badge/amd64-yes-green.svg

## Requirements

Requires MariaDB addon or an external database server, it is not included with this addon.
If using the Home Assistant MariaDB addon, simply configure it to create a wavelog database
and wavelog user.

## Installation

Add this repository as a custom repository in the Home Assistant addon store, and then install the addon. Once started, the installer will be available on port 8086. After the initial installation, the wizard should remain locked even if the addon is uninstalled and reinstalled unless the configuration is deleted from the `/addon_config` folder (available in HA thru visual studio server)

## Updates

Rebuilding the container will pull the latest upstream wavelog container and upgrade the software, or wait for this repository to be updated with a new version number for the automated update to work.

## Backups

It's a good idea to back up both the sql database and the configuration files, as well as dumping ADIF contacts. Check the wavelog documentation for how to dump the adif data with a curl.

## Issues

I've found the database migration install step to fail sometimes after dropping and recreating the database.
