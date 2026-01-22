# ambxst-uki-splash-screen
ambxst splash-screen while booting. Will only work on systems running a **U**nified **K**ernel **I**mage and systemd-boot. It should also work an 'regular' systems! There are plenty of tutorials out there :)

1. download splash-arch.bmp
2. add this to `/etc/mkinitcpio.d/linux[-zen].preset`*  :

`default_options="--splash /usr/share/systemd/bootctl/splash-arch.bmp"`

3. move the splash-arch.bmp to said location
4. `sudo mkinitcpio -P`

*name depends on your kernel type

Preview:
![splash-screen](splash-arch.bmp)