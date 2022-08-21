# Using dynamic buffering on Debian of Debian testing

[Related News](https://www.phoronix.com/news/GNOME-Triple-Buffering-2x)

The dynamic buffering allows the animation of GNOME desktop up to 120fps on some devices, which can significantly reduce visible lag.

## Build (Not Required)

1. Get source of mutter

    `apt source mutter`

2. Get dynamic buffering patch from AUR

    [From There](https://aur.archlinux.org/packages/mutter-dynamic-buffering)

3. Apply patch and build packages

    [Follow This](https://medium.com/@da.mikulasova/apply-patch-for-debian-package-968b8929fda)

4. Install builted packages

    Only need gir1.2-mutter-10_42.3-2_amd64.deb, libmutter-10-0_42.3-2_amd64.deb, mutter_42.3-2_amd64.deb and mutter-common_42.3-2_all.deb.
