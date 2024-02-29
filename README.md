# My fork of the davfs2 aur package

---
The problem with the AUR package is that it requires neon. neon from the arch repositories is not built with SSL-support enabled. thus you need to buiild a compatible version of neon (I use 0.32.5) with SSL-Support enabled. Then if you try to install the davfs2 from the AUR it tries to pull neon, which overwrites your custom installation. Removing neon as a dependency from the PKGBUILD has solved this issue for me. Everything works fine now.
