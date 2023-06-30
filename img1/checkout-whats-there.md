
```bash
root@imx8mmevk:~# cat /etc/os-release
ID=fsl-imx-xwayland
NAME="NXP i.MX Release Distro"
VERSION="5.15-kirkstone (kirkstone)"
VERSION_ID=5.15-kirkstone
PRETTY_NAME="NXP i.MX Release Distro 5.15-kirkstone (kirkstone)"
DISTRO_CODENAME="kirkstone"
```

```bash
root@imx8mmevk:~# cat /etc/issue
NXP i.MX Release Distro 5.15-kirkstone \n \l
```

https://www.variscite.com/software-releases/new-release-yocto-kirkstone-5-15-2-0-x-v1-0-for-i-mx8m-plus-modules/

```bash
root@imx8mmevk:~# fbset

mode "1024x600"
    geometry 1024 600 1024 600 32
    timings 0 0 0 0 0 0 0
    accel true
    rgba 8/16,8/8,8/0,0/0
endmode
```
```bash
root@imx8mmevk:~# lsmod
Module                  Size  Used by
```