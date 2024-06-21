# Charmed PgBouncer Snap
[![Release to Snap Store](https://github.com/canonical/charmed-pgbouncer-snap/actions/workflows/release.yaml/badge.svg)](https://github.com/canonical/charmed-pgbouncer-snap/actions/workflows/release.yaml)

This repository contains the packaging metadata for creating a snap of PgBouncer built from the official Ubuntu repositories.  For more information on snaps, visit [snapcraft.io](https://snapcraft.io/). 

## Installing the Snap
The snap can be installed directly from the Stap Store.  Follow the link below for more information.
<br>

[![Get it from the Snap Store](https://snapcraft.io/static/images/badges/en/snap-store-black.svg)](https://snapcraft.io/charmed-pgbouncer)

## Building the Snap
### Clone Repository
```bash
git clone git@github.com:canonical/charmed-pgbouncer-snap.git
cd charmed-pgbouncer-snap
```
### Installing and Configuring Prerequisites
```bash
sudo snap install snapcraft
sudo snap install lxd
sudo lxd init --auto
```
### Packing and Installing the Snap
```bash
snapcraft pack
sudo snap install ./charmed-pgbouncer*.snap --devmode
```

## License
The PgBouncer Snap is free software, distributed under the Apache
Software License, version 2.0. See
[LICENSE](https://github.com/canonical/charmed-pgbouncer-snap/blob/1/edge/LICENSE)
for more information.
