
<div align="center">
  <img src="./static/logo.png" alt="logo" width="150" height="150">
</div>

# live-build configuration for Debian loong64 images

Total downloads：![](https://gh-down-badges.linkof.link/elysia-best/debian-live-build-loong64)

Have a look at [Debian Live Manual](https://live-team.pages.debian.net/live-manual/html/live-manual/index.en.html) for explanations on how to use this repository.

# Download prebuilt images

**Nightly Builds**: Download the latest prebuilt image from [here](https://nightly.link/elysia-best/debian-live-build-loong/workflows/build/master/Debian%20loong64%20live%20cd.zip).

**Latest Release**: See the release page for details.
# Build images

## Install dependencies

```bash
sudo apt install sudo git fakeroot debootstrap debian-cd simple-cdd xorriso squashfs-tools mtools curl libxml2-utils -y
curl -fsSL https://salsa.debian.org/-/project/100777/uploads/67ffd6906e0fd6ea39607917e8f78655/live-build_20251022_all.deb -o live-build.deb
sudo apt install -y ./live-build.deb
rm live-build.deb
```

## Clone this repository

```bash
git clone https://github.com/elysia-best/debian-live-build-loong.git
cd debian-live-build-loong
```

## Build images

```bash
sudo bash ./build.sh
```

Built images will be in `./images/`.

# Sponsor

If you like this project, you can sponsor me on [buymeacoffee](https://buymeacoffee.com/elysia.best) with any amount you want.

# License

This project is licensed under the Attribution-ShareAlike 4.0 International.
