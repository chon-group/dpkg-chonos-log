# Changelog
## 1.3 (2023-09-16)
Solving problem of adption of [PEP 668 (Python Enhancement Proposal – Marking Python base environments as “externally managed”)](https://peps.python.org/pep-0668/) in differents versions of Linux Distribution that has been broken the instalation os chonos-log. 

For example:
```sh
    sudo pip3 install any --break-system-packages
``` 

+ Debian >= 12: Implements the PEP668, so in the instalation is necessary set the --break-system-packages 

+ Debian <= 11: Not implements the PEP668, so in the instalation the option --break broken the installer like below:

![img](.imgs/debian11-error.png)

## 1.2.6 (2023-09-13)
### Solving [Issue 14 of ChonIDE](https://github.com/chon-group/chonIDE/issues/14)
- Forcing python3-pip to install wtee
## 1.2.5 (2023-05-18)
### Bug
- Adding Python 3.11 packages, in Debian 12.
## 1.2.0 (2023-04-30)
### Enhancements
- It adding an elegant way for other services to inform events.
## 1.0.0 (2023-04-23)
### Enhancements
- It implements the chonos-log as a background daemon.