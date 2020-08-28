# OC-Configs
This repo has a couble of configs built by ARhackintosh to make config setup easier for new users.

these configs are missing platform info and have incomplete settings.
you will need to edit the config before using it.
of course you will need to add your kexts and ssdt/dsdt to config too.

## missing info:
- **ivy-bridge**:
    - if you have a 6 series mobo you need to edit [DeviceProperties-Add](https://dortania.github.io/OpenCore-Install-Guide/config.plist/ivy-bridge.html#add-2)
    - this config is setup for HD4000 you need to change the id if you have a diffrent gpu
    - if you are missing some bios options you need to edit [Kernel-Quirks](https://dortania.github.io/OpenCore-Install-Guide/config.plist/ivy-bridge.html#quirks-3)
    - to change bootargs edit [NVRAM-Add](https://dortania.github.io/OpenCore-Install-Guide/config.plist/ivy-bridge.html#add-4)
    - you have to change the SMBios and add all the missing info(mlb,rom,product,serial) in [Platforminfo](https://dortania.github.io/OpenCore-Install-Guide/config.plist/ivy-bridge.html#platforminfo)
    - if you use an hp motherboard, you also have to enable unblockfsconnect in [UEFI-Quirks](https://dortania.github.io/OpenCore-Install-Guide/config.plist/ivy-bridge.html#quirks-4)