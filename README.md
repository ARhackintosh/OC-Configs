# OC-Configs
<div dir="rtl">

هذا المشروع هو عباره عن عينه كونفقات غير كامله, لتجعل عمليه انشاء كونفقات اوبن كور اسهل للمستخدم المبتدء.
هذه الكونفقات تنقصها اشياء كثيره تخص الجهاز 
بحيث نقوم بوضع الاعدادات العامه فقط وترك الاعدادات المخصصه للجهاز للمستخدم
الاعدادات الناقصه, وما يجب تغيير ستكون موجوده في [الاصدار الثاني من شرح تثبيت الهاكنتوش](https://github.com/ARhackintosh/ARtutorial)

</div>

## English
These are sample configs built by ARhackintosh to make config setup easier for new users.

these configs are missing platform info and only have general settings.
any settings which depend on hardware other than cpu gen (bios settings, mobo type, etc..) are on the user to complete.

you will need to add your kexts and ssdt/dsdt to the config too.

## settings to change:

### Desktops:
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

- **Comet Lake**
    - if you have a z390 mobo you need to enable ProtectUefiServices in [Booter-Quirks](https://dortania.github.io/OpenCore-Install-Guide/config.plist/coffee-lake.html#quirks-2)
    - if you have missing bios options you have to edit [kernel-quirks](https://dortania.github.io/OpenCore-Install-Guide/config.plist/coffee-lake.html#add-2)
    - to change bootargs edit [NVRAM-Add](https://dortania.github.io/OpenCore-Install-Guide/config.plist/coffee-lake.html#add-4)
    - you have to change the SMBios, and add all the missing info(mlb,rom,product,serial) in [Platforminfo](https://dortania.github.io/OpenCore-Install-Guide/config.plist/coffee-lake.html#platforminfo)
    - if you use an hp motherboard, you also have to enable unblockfsconnect in [UEFI-Quirks](https://dortania.github.io/OpenCore-Install-Guide/config.plist/coffee-lake.html#quirks-4)

### Laptops

- **ivy-bridge**:
    - DeviceProperties-Add](https://dortania.github.io/OpenCore-Install-Guide/config-laptop.plist/ivy-bridge.html#add-2):
        - you need to add device id depending on your display's res
        - if you have a device with a 6th gen mobo you have to change the IMEI id
    - if you are missing some bios options you need to edit [Kernel-Quirks](https://dortania.github.io/OpenCore-Install-Guide/config-laptop.plist/ivy-bridge.html#quirks-3)
    - to change bootargs edit [NVRAM-Add](https://dortania.github.io/OpenCore-Install-Guide/config-laptop.plist/ivy-bridge.html#add-4)
    - if your device has no Native support for nvram you should edit [NVRAM-Delete](https://dortania.github.io/OpenCore-Install-Guide/config-laptop.plist/ivy-bridge.html#delete-3)
    - you have to change the SMBios and add all the missing info(mlb,rom,product,serial) in [Platforminfo](https://dortania.github.io/OpenCore-Install-Guide/config-laptop.plist/ivy-bridge.html#platforminfo)
    - if you use an hp motherboard, you also have to enable unblockfsconnect in [UEFI-Quirks](https://dortania.github.io/OpenCore-Install-Guide/config-laptop.plist/ivy-bridge.html#quirks-4)

- **haswell**
    - you have to specify your igpu in [DeviceProperties-Add](https://dortania.github.io/OpenCore-Install-Guide/config-laptop.plist/haswell.html#add-2)
    - if you have missing bios options you have to edit [kernel-quirks](https://dortania.github.io/OpenCore-Install-Guide/config-laptop.plist/haswell.html#quirks-3)
    - to change bootargs edit [NVRAM-Add](https://dortania.github.io/OpenCore-Install-Guide/config-laptop.plist/haswell.html#add-4)
    - if your device has no Native support for nvram you should edit [NVRAM-Delete](https://dortania.github.io/OpenCore-Install-Guide/config-laptop.plist/haswell.html#delete-3)
    - you have to change the SMBios, and add all the missing info(mlb,rom,product,serial) in [Platforminfo](https://dortania.github.io/OpenCore-Install-Guide/config-laptop.plist/haswell.html#platforminfo)
    - if you use an hp motherboard, you also have to enable unblockfsconnect in [UEFI-Quirks](https://dortania.github.io/OpenCore-Install-Guide/config-laptop.plist/haswell.html#quirks-4)

- **Broadwell**
    - if you have an hd5600 [DeviceProperties-Add](https://dortania.github.io/OpenCore-Install-Guide/config-laptop.plist/broadwell.html#add-2)
        - also if you have a kernel panic you have to add some additional properties.
    - if you have missing bios options you have to edit [kernel-quirks](https://dortania.github.io/OpenCore-Install-Guide/config-laptop.plist/broadwell.html#quirks-3)
    - to change bootargs edit [NVRAM-Add](https://dortania.github.io/OpenCore-Install-Guide/config-laptop.plist/broadwell.html#add-4)
    - if your device has no Native support for nvram you should edit [NVRAM-Delete](https://dortania.github.io/OpenCore-Install-Guide/config-laptop.plist/broadwell.html#delete-3)
    - you have to change the SMBios, and add all the missing info(mlb,rom,product,serial) in [Platforminfo](https://dortania.github.io/OpenCore-Install-Guide/config-laptop.plist/broadwell.html#platforminfo)
    - if you use an hp motherboard, you also have to enable unblockfsconnect in [UEFI-Quirks](https://dortania.github.io/OpenCore-Install-Guide/config-laptop.plist/broadwell.html#quirks-4)