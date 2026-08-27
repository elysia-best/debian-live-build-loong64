
<div align="center">
  <img src="./static/logo.png" alt="logo" width="150" height="150">
</div>

# live-build configuration for Debian loong64 images

Total downloads：![](https://gh-down-badges.linkof.link/elysia-best/debian-live-build-loong64)

Have a look at [Debian Live Manual](https://live-team.pages.debian.net/live-manual/html/live-manual/index.en.html) for explanations on how to use this repository.

# Download prebuilt images

1. SourceForge： <https://sourceforge.net/projects/elysia-loongarch-debian/files/iso/>
2. My OpenList Netdisk(For CN users/推荐中国大陆用户使用)： <https://opensrc.qinyn.eu.org/lanzou/loongarch64/iso>
3. Github Release Page: Due to gh size limit, no longer upload iso to gh release.

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
