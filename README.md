Add the Public Package Signing Key to pacman

    curl -O https://sonicde-artix-unofficial.informationhouse.co.uk/sonicde-artix-unofficial-public.asc
    sudo pacman-key --add sonicde-artix-unofficial-public.asc
    sudo pacman-key --finger 8F74E8CCCB380B1D598B13C8FFA739AC998BD51A
    sudo pacman-key --lsign-key 8F74E8CCCB380B1D598B13C8FFA739AC998BD51A

Add the repo to /etc/pacman.conf

    [sonicde-artix-unofficial]
    Server = https://gripped.github.io/sonicde-artix-unofficial

A bit more info: https://forum.artixlinux.org/index.php/topic,10298

PKGBUILD's: https://github.com/gripped/sonicde-artix-unofficial-pkgbuilds

The script that builds it: https://github.com/gripped/sonicde-artix-unofficial-script
