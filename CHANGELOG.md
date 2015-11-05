# Change log

This file contains al notable changes to the bertvv.samba Ansible role.

This file adheres to the guidelines of [http://keepachangelog.com/](http://keepachangelog.com/). Versioning follows [Semantic Versioning](http://semver.org/).

## 2.0.0 - 2015-11-05

Bugfix release with changes that are not backwards compatible

### Changed

- Fixed GH-1: The variable type of `samba_load_*` is now boolean instead of string, which makes more sense. However, this change is **not backwards compatible**.
- Fixed GH-2: Restart WinBind when changing the configuration
- Updated the base box for the test environment to CentOS 7.1 ([bertvv/centos71](https://atlas.hashicorp.com/bertvv/boxes/centos71/))
- Cleaned up indentation and spaces in the configuration file template

### Removed

- The firewall configuration is no longer set by this role. This also removes the dependency on firewalld.

## 1.0.0 - 2015-03-14

First release

### Added

- Installation
- Create directories
- SELinux settings
- Configuration template with a.o. configurable print sharing, home directories, user access control
- Set user passwords

