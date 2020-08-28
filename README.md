# OC-Configs
This repo has a couble of configs built by ARhackintosh to make config setup easier for new users.

these configs are missing platform info and have incomplete settings.
you will need to edit the config before using it.
of course you will need to add your kexts and ssdt/dsdt to config too.

## settings to change:
- **ivy-bridge**:
    - if you have a 6 series mobo you need to edit [DeviceProperties-Add](https://dortania.github.io/OpenCore-Install-Guide/config.plist/ivy-bridge.html#add-2)
    - this config is setup for HD4000 you need to change the id if you have a diffrent gpu
    - if you are missing some bios options you need to edit [Kernel-Quirks](https://dortania.github.io/OpenCore-Install-Guide/config.plist/ivy-bridge.html#quirks-3)
    - to change bootargs edit [NVRAM-Add](https://dortania.github.io/OpenCore-Install-Guide/config.plist/ivy-bridge.html#add-4)
    - you have to change the SMBios and add all the missing info(mlb,rom,product,serial) in [Platforminfo](https://dortania.github.io/OpenCore-Install-Guide/config.plist/ivy-bridge.html#platforminfo)
    - if you use an hp motherboard, you also have to enable unblockfsconnect in [UEFI-Quirks](https://dortania.github.io/OpenCore-Install-Guide/config.plist/ivy-bridge.html#quirks-4)

- **haswell**
    - you have to specify how do you use the igpu in [DeviceProperties-Add](https://dortania.github.io/OpenCore-Install-Guide/config.plist/haswell.html#add-2)
    - if you have missing bios options you have to edit [kernel-quirks](https://dortania.github.io/OpenCore-Install-Guide/config.plist/haswell.html#add-2)
    - to change bootargs edit [NVRAM-Add](https://dortania.github.io/OpenCore-Install-Guide/config.plist/haswell.html#add-4)
    - you have to change the SMBios, and add all the missing info(mlb,rom,product,serial) in [Platforminfo](https://dortania.github.io/OpenCore-Install-Guide/config.plist/haswell.html#platforminfo)
    - if you use an hp motherboard, you also have to enable unblockfsconnect in [UEFI-Quirks](https://dortania.github.io/OpenCore-Install-Guide/config.plist/haswell.html#quirks-4)

- **skylake**
    - you have to specify how do you use the igpu in [DeviceProperties-Add](https://dortania.github.io/OpenCore-Install-Guide/config.plist/skylake.html#add-2)
    - if you have missing bios options you have to edit [kernel-quirks](https://dortania.github.io/OpenCore-Install-Guide/config.plist/skylake.html#add-2)
    - to change bootargs edit [NVRAM-Add](https://dortania.github.io/OpenCore-Install-Guide/config.plist/skylake.html#add-4)
    - you have to change the SMBios, and add all the missing info(mlb,rom,product,serial) in [Platforminfo](https://dortania.github.io/OpenCore-Install-Guide/config.plist/skylake.html#platforminfo)
    - if you use an hp motherboard, you also have to enable unblockfsconnect in [UEFI-Quirks](https://dortania.github.io/OpenCore-Install-Guide/config.plist/skylake.html#quirks-4)

- **kaby lake**
    - you have to specify how do you use the igpu in [DeviceProperties-Add](https://dortania.github.io/OpenCore-Install-Guide/config.plist/kaby-lake.html#add-2)
    - if you have missing bios options you have to edit [kernel-quirks](https://dortania.github.io/OpenCore-Install-Guide/config.plist/kaby-lake.html#add-2)
    - to change bootargs edit [NVRAM-Add](https://dortania.github.io/OpenCore-Install-Guide/config.plist/kaby-lake.html#add-4)
    - you have to change the SMBios, and add all the missing info(mlb,rom,product,serial) in [Platforminfo](https://dortania.github.io/OpenCore-Install-Guide/config.plist/kaby-lake.html#platforminfo)
    - if you use an hp motherboard, you also have to enable unblockfsconnect in [UEFI-Quirks](https://dortania.github.io/OpenCore-Install-Guide/config.plist/kaby-lake.html#quirks-4)

- **Coffee lake**
    - if you have a z390 mobo you need to enable ProtectUefiServices in [Booter-Quirks](https://dortania.github.io/OpenCore-Install-Guide/config.plist/coffee-lake.html#quirks-2)
    - if you have missing bios options you have to edit [kernel-quirks](https://dortania.github.io/OpenCore-Install-Guide/config.plist/coffee-lake.html#add-2)
    - to change bootargs edit [NVRAM-Add](https://dortania.github.io/OpenCore-Install-Guide/config.plist/coffee-lake.html#add-4)
    - you have to change the SMBios, and add all the missing info(mlb,rom,product,serial) in [Platforminfo](https://dortania.github.io/OpenCore-Install-Guide/config.plist/coffee-lake.html#platforminfo)
    - if you use an hp motherboard, you also have to enable unblockfsconnect in [UEFI-Quirks](https://dortania.github.io/OpenCore-Install-Guide/config.plist/coffee-lake.html#quirks-4)
