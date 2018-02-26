# linux-apparmor-patchset
Patchset for ArchLinux stock kernel for enable AppArmor

## How to use it

1. Install ASP
```sh
pacman -S asp
```

2. Get source file of linux package
```sh
asp export linux
```

3. Get patchset
```sh
git clone https://github.com/tears-of-noobs/linux-apparmor-patchset.git
```

4. Apply patchset and build kernel
```sh
cd linux
patch -p1 -i ../linux-apparmor-patchset/*.patch
makepkg
```
