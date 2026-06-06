# Changelog

The **Next** series continues development of the plugin by the original author and focuses on ongoing maintenance, reliability improvements, and compatibility with current Unraid releases.

Development of the plugin will continue with ongoing fixes, enhancements, and maintenance improvements.


## 2026.06.06

### Fixes

- Changed File Activity configuration updates from a full restart to a reload operation.
- Reload requests are now queued and consolidated, with a single reload performed after 10 seconds of inactivity. This prevents excessive reload activity when plugins such as Unassigned Devices generate multiple mount and unmount events in rapid succession.

### Enhancements

- Added a 30-second startup delay during system boot and plugin updates to allow the server and storage configuration to stabilize before File Activity begins monitoring file system activity.

## 2026.05.10

### Fixes
- Conflicts starting File Activity on boot.

## 2026.05.02

### Fixes
- Inotify starting issues on server boot.

## 2026.04.23

### Fixes
- Prevent the file var.ini missing from generating a script error email.
- Delay the start of file activity when booting up.

## 2026.04.06

### Fixes
- Improved overall reliability of File Activity monitoring by addressing logging interruptions and enhancing runtime status visibility

### Notes
- Detailed technical changes are documented in the GitHub release notes
