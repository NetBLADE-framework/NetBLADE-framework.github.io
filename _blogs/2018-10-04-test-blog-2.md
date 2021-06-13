---
title:  "Setup wake on LAN on local server"
search: true
categories: 
  - Linux
  - Networking
last_modified_at: 2018-09-27T08:05:34-05:00
header:
  teaser: /assets/images/blog/setup-wake-on-lan.jpg
---

![WoLAN](/assets/images/blog/setup-wake-on-lan.jpg)

Why Wake on LAN? Wake on LAN is program to wake a system which is under deep sleep. That is, the system is shut down with power access. A system with an enabled Wake-on-LAN feature can be turned on using a special packet. This special packet is sent by the client remotely.

To implement Wake-On-LAN on the server, we need to install ethtool on our server and wakeonlan commanline program on our personal system.

First we will setup our server:-

1. Enable wake-on-LAN on BIOS settings. Enter into BIOS and search for wake on LAN and enable it.
   Make sure the ethernet cable connect from the server to the switch or router has all the 8 pins connected. This is because the magic packet is sent via a dedicatd pin, usually last 2 pins.
   Install ethtool into the server.

   (Ubuntu / Debian)

   ```yaml
   $ sudo apt install ethtool
   ```

   (Fedora)

   ```yaml
   $ sudo dnf install ethtool
   ```

   (RHEL / CentOS)

   ```yaml

   $ sudo yum install ethtool
   ```

2. Now let's find the name of ethernet port present in the system. This command will also reveal the mac address.

   ```yaml
   $ ip a
   ```

   The above command will output the ethernet port name (Lets consider the ethernet name to be enp9s0).
3. Let's check if ethtool detects the port.

   ```yaml
   $ sudo ethtool enp9s0
   ```

4. Now, let's activate wake on lan.

   ```yaml
   $ sudo ethtool -s enp8s0 wol g
   ```

5. Now, we will setup wake on client on your system. i.e, the system that will be used to wake the server.

   (Ubuntu / Debian)

   ```yaml
   $ sudo apt install etherwake
   ```

   (Mac)

   ```yaml
   $ brew install wakeonlan
   ```

   (Fedora / RHEL / CentOS)

   ```yaml
   $ wget http://gsd.di.uminho.pt/jpo/software/wakeonlan/downloads/wakeonlan-0.41-0.fdr.1.noarch.rpm 
   $ rpm -Uvh wakeonlan-0.41-0.fdr.1.noarch.rpm
   ```

Now, we can wake the system using the wakeonlan command.
Execute the following command.

```yaml
   $ wakeonlan mac-address
```

The above command will wake your system.