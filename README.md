# Mullvad VPN for Void Linux

This repository provides an [xbps-src](https://github.com/void-linux/void-packages)
template, runit service, and install/remove hooks for running
[Mullvad VPN](https://github.com/mullvad/mullvadvpn-app) on Void Linux.

## Installation

### Build with xbps-src

```sh
git clone https://github.com/void-linux/void-packages.git
cd void-packages
./xbps-src binary-bootstrap
```

Clone this repository and copy the `mullvadvpn-void/srcpkgs/mullvad-vpn` folder
into `void-packages/srcpkgs`, then run:

```sh
./xbps-src pkg mullvad-vpn
sudo xbps-install --repository=hostdir/binpkgs mullvad-vpn
```
