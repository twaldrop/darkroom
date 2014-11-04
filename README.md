# Darkroom - a tool to build openstack images via packer

Darkroom uses Packer to build OpenStack images inside your OpenStack environment

# Installation

```bash
git clone git@github.com:blueboxgroup/darkroom.git
cd darkroom
python config.py install
```

# Pre-Requisites

Access to an OpenStack cluster with the resources to create a new instance with 8GB memory.

# Setup

Source your OpenStack credentials:
```bash
source ~/stackrc
```

Edit config.yml with your desired image settings.

```bash
name: centos5.11
distro: centos
version: '5.11'
kickstart_path: kickstarts/kickstart.centos5.cfg
```

kickstart_path - usethe path to the kickstart file for your desired distro

# Supported Distros

Centos 5.11

```bash
distro: centos
version: '5.11'
```
Scientific Linux 6

```bash
distro: sl6
version: '5.11'
```

======================================================


