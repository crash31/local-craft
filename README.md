# Craft Dev Environment
> Get to coding, nerds.

This is a development boilerplate for a project in [Craft CMS](https://craftcms.com/) utilizing [Docksal](https://docksal.io/) for a local server environment.

This is just a vanilla boilerplate for Craft. In future versions there will be more development environments set up, hopefully utilizing npm and webpack for package management and script bundling respectively.

---

# Set up the Local Server

## System Requirements

#### CPU

- (Mac) Must be a 2010 or newer model
- (PC) Your CPU should support hardware VT-x/AMD-V virtualization and it should be [enabled in BIOS](https://access.redhat.com/documentation/en-US/Red_Hat_Enterprise_Linux/6/html/Virtualization_Administration_Guide/sect-Virtualization-Troubleshooting-Enabling_Intel_VT_and_AMD_V_virtualization_hardware_extensions_in_BIOS.html)

#### RAM

- (Mac/Win) Workstation with 4GB is required (8GB recommended)
- (Linux) no minimum requirement (4GB recommended)

#### Software

- 64-bit OS is required for all platforms
- (Mac) OS X El Capitan 10.11 or newer
- (Mac) VirtualBox prior to version 4.3.30 must NOT be installed
- (Win) Windows 7 or newer
- (Linux) Ubuntu Linux 14.04 or newer (or it's derivatives) with Linux kernel 3.10 or newer

Refer to the [environment setup instructions for further steps](https://docs.docksal.io/en/latest/getting-started/env-setup/)

## Environment Set Up

_See the [Docksal documentation](https://docs.docksal.io/) for more details_

#### Installing Docksal on macOS

1. Install Docksal

  `curl -fsSL get.docksal.io | sh`

2. Create and start the vm

  `fin vm start`

  [Help, my VM did not start!](https://docs.docksal.io/en/latest/troubleshooting/#failed-creating-docksal-virtual-machine)

3. Congratulations!

  You are done with the one time environment installation. Now you can [configure your project] to use Docksal or create a new pre-configured project with `fin project create`.

## Project Installation

1. Clone the project from the repository into your desired directory.

  `git clone [this git url]`

2. cd into the project directory you just cloned

  `cd [project name]`

3. Start the Docksal environment outlined in the project's .docksal directory.

  `fin start` or `fin up`

  _If this does not work see the [Docksal docs](https://docs.docksal.io/) for troubleshooting_

4. In the browser, go to [project name].docksal in order to view your project on the front end.

  > eg. _mycraft.docksal_

  In order to install Craft, go to `mycraft.docksal/admin` which should redirect you to the installation page for this project.

5. All of the editable files for this project are in the `docroot` directory for this project. Code away.
