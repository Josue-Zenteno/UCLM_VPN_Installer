# UCLM VPN Linux Installer

## Developers
* **Josue Carlos Zenteno Yave**

## Automatic Installation

**1. Depending on your Operative System you should use one of these options:**
    [Red Hat, Fedora, CentOS] => ```-Rh```
    [Debian, Ubuntu] => ```-Deb```
    [Arch] => ```-Ar```

**2. Execute:**
```./install_vpn <OS>```

## How to use the VPN

**1. Execute:**
    ```sudo openconnect --protocol=gp portal.vpn.uclm.es```

## Manual Installation

**1. Download and extract:**
    https://launchpad.net/ubuntu/+archive/primary/+sourcefiles/openconnect/8.02-1build1/openconnect_8.02.orig.tar.gz

**2. Install dependences:**
```sudo apt-get install build-essential gettext autoconf automake libproxy-dev libxml2-dev libtool vpnc-scripts pkg-config zlib1g-dev```

**3. Depending on your OS execute one of these commands:**
    [Red Hat, Fedora, CentOS] => ```sudo apt-get install openssl-devel```
    [Debian, Ubuntu] => ```sudo apt-get install libssl-dev```
    [Arch] => ```sudo apt-get install openssl```

**4. Into the openconnect folder execute:**
    ```./configure```

**5. Finally execute:**
    ```sudo make install && sudo ldconfig```
