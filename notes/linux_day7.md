# Linux Day 7 - Core Concepts

## Root vs sudo
Root is the usperuser with unrestriced access.
Sudo allows temporary execution of commands with elevated privileges.

## Services and Security
Serices should not run as root to reduce security risks.
Each service should run as a limited user.

## Troubleshooing
Logs are the first place to look when something fails.
journalctl and /var/log are key locations.

## Linux Services
A service is a long-running background process managed by systemctl.
Example include SSH and web servers
