# Singularity OS

Build system for the Singularity OS root and kernelcache images.

## Prerequisites

On Ubuntu/Debian:

```bash
sudo apt-get install -y \
  build-essential gcc g++ make \
  bc bison flex libssl-dev libelf-dev \
  libncurses-dev wget rsync cpio \
  xz-utils gzip bzip2 patch perl python3 \
  git unzip erofs-utils cryptsetup-bin \
  systemd-boot binutils
```
On Arch Linux

With yay (or paru):

```bash
yay -S base-devel openssl elfutils ncurses bc bison flex wget rsync cpio \
  xz-utils gzip bzip2 patch perl python3 git unzip cryptsetup binutils \
  systemd erofs-utils
```

## Build

```bash
./scripts/prepare.sh
./scripts/compile.sh
./scripts/package.sh
```
