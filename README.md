![GitHub release (latest by date)](https://img.shields.io/github/v/release/fossee/esim?color=blueviolet)
![GitHub](https://img.shields.io/github/license/fossee/esim?color=blue)
![Python](https://img.shields.io/badge/python-v3.6+-blue.svg)
[![PEP8](https://img.shields.io/badge/code%20style-pep8-orange.svg)](https://www.python.org/dev/peps/pep-0008/)
![Travis (.com)](https://img.shields.io/travis/com/Eyantra698Sumanto/eSim)
[![Documentation Status](https://readthedocs.org/projects/esim/badge/?version=latest)](https://esim.readthedocs.io/en/latest/?badge=latest)
[![GitHub forks](https://img.shields.io/github/forks/fossee/esim)](https://github.com/fossee/esim/network)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat)](https://github.com/fossee/esim)
![GitHub contributors](https://img.shields.io/github/contributors/fossee/esim)
#UPdated By Vanshika MOtwani(31st Jan,2026)

[eSim](https://esim.fossee.in/) is an open source EDA tool for circuit design, simulation, analysis and PCB design, developed by [FOSSEE Team](https://www.fossee.in/) at [IIT Bombay](https://www.iitb.ac.in/).
It is an integrated tool build using open source softwares such as KiCad, Ngspice and GHDL.

## Releases and Installation
eSim is released for the following distributions (operating systems):
* Ubuntu 22.04, 23.04, 24.04 LTS versions.
* Microsoft Windows 8, 10 and 11.
## Tested Environment

This project was tested and verified on the following system:
- OS: Ubuntu 25.04 (VirtualBox VM)
- Architecture: x86_64
- Python: 3.x
- SSH-based GitHub authentication

All setup steps were executed successfully on this environment.
Jan 31,2026)

To use eSim on your machine having above distributions, please refer to link [here](https://esim.fossee.in/downloads) for installation and other guidelines.
## Common Issues and Fixes

### SSH Permission Denied (publickey)
If you face SSH authentication issues while pushing to GitHub:

- Ensure SSH key is generated using:
  `ssh-keygen -t ed25519`
- Add the public key (`id_ed25519.pub`) to GitHub → Settings → SSH keys
- Start ssh-agent and add key:
  `eval "$(ssh-agent -s)"`
 
  `ssh-add ~/.ssh/id_ed25519`
- Test connection:
  `ssh -T git@github.com`

This project was successfully pushed using SSH authentication.

> Note for other distributions: You can refer [`installers`](https://github.com/fossee/eSim/tree/installers) branch for documentation on packaging (for above mentioned distributions) to build installers for your operating system in a similar way. For providing your build, please check the `Contribution` section mentioned below.

## Features
* An open-source EDA tool.
* Perform Circuit Design.
* Perform Simulation.
* Perform Layout Design.
* Model and Subcircuit builder.
* Support for Mixed-Signal Simulations including Microcontrollers.
* eSim has been successfully ported to low cost FOSSEE [laptop](https://laptop.fossee.in/)

##  Known Limitation

Python 3.13 on Ubuntu 25.04 is currently incompatible with eSim-2.5
due to deprecated setup.py workflows and unsupported dependencies.

No forced downgrade was attempted to preserve system stability.

## Open-Source Softwares Used
* [Python](https://www.python.org/)
* [KiCad](https://www.kicad.org/)
* [NGHDL](https://github.com/fossee/nghdl/)
* [Makerchip](https://www.makerchip.com/)
* [SkyWater SKY130 PDK](https://skywater-pdk.rtfd.io/)

## eSim Manual
To know everything about eSim, how it works and it's feature please download the manual from [here](https://static.fossee.in/esim/manuals/eSim_Manual_2.5.pdf)

## Contact
For any queries regarding eSim please write us on at this [email address](mailto:contact-esim@fossee.in).

Other Contact Details are available [here](https://esim.fossee.in/contact-us).

## Contribution
Please refer [here](https://github.com/FOSSEE/eSim/blob/master/CONTRIBUTION.md) for further details.

## License
It is developed by FOSSEE Team at IIT Bombay and is released under GNU GPL License.
---
Maintained and tested by **Vanshika Motwani** (2026)
> Recent contributions include Ubuntu 25.04 setup troubleshooting.
> See [CONTRIBUTION.Md](CONTRIBUTION.md) for details.
