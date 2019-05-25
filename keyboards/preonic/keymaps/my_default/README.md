# README

## Installation note (Arch)

`arm-none-eabi-gcc` must be downgraded to version 7.3. Run the following:

```bash
sudo pacman -R arm-none-eabi-gcc
aurman -S arm-none-eabia-gcc73-linaro
sudo ln -s /usr/bin/arm-none-eabi-gcc-7.3 /usr/bin/arm-none-eabi-gcc
```

## Make firmware
After which you should be able to build the default keymap with:

```bash
make preonic/rev3:default
```

## Flash keyboard

```
make preonic/rev3:default:dfu-util
```

