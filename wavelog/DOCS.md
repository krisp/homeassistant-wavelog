# Home Assistant Add-on: Wavelog

This addon installs the latest Wavelog release. 

## Requirements

Requires MariaDB addon or an external database server, it is not included with this addon.
If using the Home Assistant MariaDB addon, simply configure it to create a wavelog database
and wavelog user.

## Installation

Copy the source to the addons folder on homeassistant. It should then be available to install
from `Settings -> Addons -> Addon Store`. After the first install, navigate to port 8086 on
the home assistant server and run through the install wizard. 

## Updates

Rebuilding the container will pull the latest upstream wavelog container and upgrade the software.
