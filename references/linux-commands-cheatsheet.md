# Linux commands cheat sheet

Examples use common GNU/Linux tools. Options and availability may differ across distributions and shells. Read a command's manual page before using unfamiliar flags.

## Files and directories

| Task | Example |
| --- | --- |
| Show current directory | `pwd` |
| List files, including hidden | `ls -la` |
| Change directory | `cd path/to/folder` |
| Create directory | `mkdir -p new/folder` |
| Copy or move a file | `cp source destination` / `mv source destination` |
| Read a file | `less file.txt` / `cat file.txt` |

## Permissions

| Task | Example |
| --- | --- |
| Inspect permissions | `ls -l` |
| Change file mode | `chmod 640 file` |
| Change owner (admin) | `sudo chown user:group file` |

Use the least access required. `sudo` runs a command with elevated privileges; understand the command before using it.

## Processes, network, and disk

| Task | Example |
| --- | --- |
| List processes | `ps aux` |
| View resource usage | `top` |
| Disk space | `df -h` |
| Directory size | `du -sh path` |
| Show interfaces/routes | `ip addr` / `ip route` |
| Test DNS lookup | `getent hosts example.com` |

## Packages and archives

Package managers differ: Debian/Ubuntu commonly use `apt`; Fedora uses `dnf`; Arch uses `pacman`. Consult your distribution's docs before installing or updating packages.

```sh
tar -czf archive.tar.gz folder/
tar -xzf archive.tar.gz
```

Avoid extracting untrusted archives into sensitive locations.

## System information

```sh
uname -a
cat /etc/os-release
```

Further reading: [Linux man-pages](https://www.kernel.org/doc/man-pages/) and [Ubuntu help](https://help.ubuntu.com/).
