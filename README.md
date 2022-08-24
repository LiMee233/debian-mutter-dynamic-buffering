# Using dynamic buffering on GNOME of Debian testing

[Related News](https://www.phoronix.com/news/GNOME-Triple-Buffering-2x)

The dynamic buffering allows the animation of GNOME desktop up to 120fps on some devices, which can significantly reduce visible lag.

## Build (Not Required)

1. Get source of mutter

    `apt source mutter`

2. Get dynamic buffering patch from AUR

    [From There](https://aur.archlinux.org/packages/mutter-dynamic-buffering)

3. Apply patch and build packages

    [Follow This](https://medium.com/@da.mikulasova/apply-patch-for-debian-package-968b8929fda)

    The following modifications are required for a successful build:

    1. Delete ` a/` and ` b/` in patch file from AUR `mr1441.patch`.

    2. Delete file: `mutter-42.4/debian/source/format`.

    3. Delete files: `mutter-42.4/debian/*.symbols`

4. Install builted packages

    In the output folder, Only need libmutter-10-0_42.4-2_amd64.deb and mutter_42.4-2_amd64.deb.
