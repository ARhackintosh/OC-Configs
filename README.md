# OC-Configs

<div dir="rtl">

## توقف الدعم
اصدار V2.8-Big Sur من شرح الهاكنتوش, سيعتمد على بناء الكونفقات مباشره من السامبل.

جاء هذا القرار لتسريع عمليه تحديث الشرح و تخفيف الحمل على الفريق.
ولستريع وتيره صدور التحديثات.
اخر اصدار يستخدم OC-Configs هو [V2.7.1-Big Sur](https://github.com/ARhackintosh/ARtutorial/releases/tag/V2.7.1)+
اخر اصدار من OC-Configs سيكون V1.6.1-April.
في حاله كنت تريد تكمله المشروع, يمكنك اشتقاق المشروع, مع ابقاء ترخيص AGPLv3

</div>

## deprecation notice

our arabic hackintosh guide [ARtutorial](https://github.com/ARhackintosh/ARtutorial) in version V2.8-Big Sur, will follow dortania's way in creating configs from the offical opencore sample.
this decision came from the need to make the update process simpler and easier for the maintainer(s) of the project, and to improve the speed at which updates are released.
the last version to use OC-Configs is [V2.7.1-Big Sur](https://github.com/ARhackintosh/ARtutorial/releases/tag/V2.7.1)
OC-Configs V1.6.1 is the last update to be released.  its built for 0.6.8 with XHCIportlimit disabled for 11.3 compatiblity
if you want to continue the project, you are welcome to fork the repo under the AGPLv3 license

<div dir="rtl">

هذا المشروع هو عباره عن عينه كونفقات غير كامله, لتجعل عمليه انشاء كونفقات اوبن كور اسهل للمستخدم المبتدء.
هذه الكونفقات تنقصها اشياء كثيره تخص الجهاز 
بحيث نقوم بوضع الاعدادات العامه فقط وترك الاعدادات المخصصه للجهاز للمستخدم
الاعدادات الناقصه, وما يجب تغيير ستكون موجوده في [الاصدار الثاني من شرح تثبيت الهاكنتوش](https://github.com/ARhackintosh/ARtutorial)

</div>

## English
These are Template configs built by ARhackintosh to make config setup easier for new users.

these configs are missing platform info and only have general settings.
any settings which depend on hardware other than cpu gen (bios settings, mobo type, etc..) are on the user to complete.

you will need to add your kexts and ssdt/dsdt to the config too.

## settings to change:

### Desktops

#### Ivy Bridge
- if you have a 6 series mobo you need to edit [DeviceProperties-Add](https://dortania.github.io/OpenCore-Install-Guide/config.plist/ivy-bridge.html#add-2)
- this config is setup for HD4000 you need to change the id if you have a different gpu
- if you are missing some bios options you need to edit [Kernel-Quirks](https://dortania.github.io/OpenCore-Install-Guide/config.plist/ivy-bridge.html#quirks-3)
- to change bootargs edit [NVRAM-Add](https://dortania.github.io/OpenCore-Install-Guide/config.plist/ivy-bridge.html#add-4)
- you have to change the SMBios and add all the missing info(mlb,rom,product,serial) in [Platforminfo](https://dortania.github.io/OpenCore-Install-Guide/config.plist/ivy-bridge.html#platforminfo)
- if you use an hp motherboard, you also have to enable unblockfsconnect in [UEFI-Quirks](https://dortania.github.io/OpenCore-Install-Guide/config.plist/ivy-bridge.html#quirks-4)

#### Haswell
- you have to specify how do you use the igpu in [DeviceProperties-Add](https://dortania.github.io/OpenCore-Install-Guide/config.plist/haswell.html#add-2)
- if you have missing bios options you have to edit [kernel-quirks](https://dortania.github.io/OpenCore-Install-Guide/config.plist/haswell.html#add-2)
- to change bootargs edit [NVRAM-Add](https://dortania.github.io/OpenCore-Install-Guide/config.plist/haswell.html#add-4)
- you have to change the SMBios, and add all the missing info(mlb,rom,product,serial) in [Platforminfo](https://dortania.github.io/OpenCore-Install-Guide/config.plist/haswell.html#platforminfo)
- if you use an hp motherboard, you also have to enable unblockfsconnect in [UEFI-Quirks](https://dortania.github.io/OpenCore-Install-Guide/config.plist/haswell.html#quirks-4)

#### Skylake
- you have to specify how do you use the igpu in [DeviceProperties-Add](https://dortania.github.io/OpenCore-Install-Guide/config.plist/skylake.html#add-2)
- if you have missing bios options you have to edit [kernel-quirks](https://dortania.github.io/OpenCore-Install-Guide/config.plist/skylake.html#add-2)
- to change bootargs edit [NVRAM-Add](https://dortania.github.io/OpenCore-Install-Guide/config.plist/skylake.html#add-4)
- you have to change the SMBios, and add all the missing info(mlb,rom,product,serial) in [Platforminfo](https://dortania.github.io/OpenCore-Install-Guide/config.plist/skylake.html#platforminfo)
- if you use an hp motherboard, you also have to enable unblockfsconnect in [UEFI-Quirks](https://dortania.github.io/OpenCore-Install-Guide/config.plist/skylake.html#quirks-4)

#### Kaby Lake
- you have to specify how do you use the igpu in [DeviceProperties-Add](https://dortania.github.io/OpenCore-Install-Guide/config.plist/kaby-lake.html#add-2)
- if you have missing bios options you have to edit [kernel-quirks](https://dortania.github.io/OpenCore-Install-Guide/config.plist/kaby-lake.html#add-2)
- to change bootargs edit [NVRAM-Add](https://dortania.github.io/OpenCore-Install-Guide/config.plist/kaby-lake.html#add-4)
- you have to change the SMBios, and add all the missing info(mlb,rom,product,serial) in [Platforminfo](https://dortania.github.io/OpenCore-Install-Guide/config.plist/kaby-lake.html#platforminfo)
- if you use an hp motherboard, you also have to enable unblockfsconnect in [UEFI-Quirks](https://dortania.github.io/OpenCore-Install-Guide/config.plist/kaby-lake.html#quirks-4)

#### Coffee Lake
- you have to specify how do you use the igpu in [DeviceProperties-Add](https://dortania.github.io/OpenCore-Install-Guide/config.plist/coffee-lake.html#add-2)
- if you have a z390 mobo you need to enable ProtectUefiServices in [Booter-Quirks](https://dortania.github.io/OpenCore-Install-Guide/config.plist/coffee-lake.html#quirks-2)
- if you have missing bios options you have to edit [kernel-quirks](https://dortania.github.io/OpenCore-Install-Guide/config.plist/coffee-lake.html#add-2)
- to change bootargs edit [NVRAM-Add](https://dortania.github.io/OpenCore-Install-Guide/config.plist/coffee-lake.html#add-4)
- you have to change the SMBios, and add all the missing info(mlb,rom,product,serial) in [Platforminfo](https://dortania.github.io/OpenCore-Install-Guide/config.plist/coffee-lake.html#platforminfo)
- if you use an hp motherboard, you also have to enable unblockfsconnect in [UEFI-Quirks](https://dortania.github.io/OpenCore-Install-Guide/config.plist/coffee-lake.html#quirks-4)

#### Comet Lake
- you have to specify how do you use the igpu in [DeviceProperties-Add](https://dortania.github.io/OpenCore-Install-Guide/config.plist/comet-lake.html#add-2)
- if you have a z390 mobo you need to enable ProtectUefiServices in [Booter-Quirks](https://dortania.github.io/OpenCore-Install-Guide/config.plist/coffee-lake.html#quirks-2)
- if you have missing bios options you have to edit [kernel-quirks](https://dortania.github.io/OpenCore-Install-Guide/config.plist/coffee-lake.html#add-2)
- to change bootargs edit [NVRAM-Add](https://dortania.github.io/OpenCore-Install-Guide/config.plist/coffee-lake.html#add-4)
- you have to change the SMBios, and add all the missing info(mlb,rom,product,serial) in [Platforminfo](https://dortania.github.io/OpenCore-Install-Guide/config.plist/coffee-lake.html#platforminfo)
- if you use an hp motherboard, you also have to enable unblockfsconnect in [UEFI-Quirks](https://dortania.github.io/OpenCore-Install-Guide/config.plist/coffee-lake.html#quirks-4)

### Laptops

**notice: we don't offer support for dgpus on laptops, these configs have the -wegnoegpu bootarg added.**

#### Ivy Bridge
- [DeviceProperties-Add](https://dortania.github.io/OpenCore-Install-Guide/config-laptop.plist/ivy-bridge.html#add-2):
    - you need to add device id depending on your display's res
    - if you have a device with a 6th gen mobo you have to change the IMEI id
- if you are missing some bios options you need to edit [Kernel-Quirks](https://dortania.github.io/OpenCore-Install-Guide/config-laptop.plist/ivy-bridge.html#quirks-3)
    - if you have an hp laptop you may enable LapicKernelPanic
- to change bootargs edit [NVRAM-Add](https://dortania.github.io/OpenCore-Install-Guide/config-laptop.plist/ivy-bridge.html#add-4)
- if your device has no Native support for nvram you should edit [NVRAM-Delete](https://dortania.github.io/OpenCore-Install-Guide/config-laptop.plist/ivy-bridge.html#delete-3)
- you have to change the SMBios and add all the missing info(mlb,rom,product,serial) in [Platforminfo](https://dortania.github.io/OpenCore-Install-Guide/config-laptop.plist/ivy-bridge.html#platforminfo)
- if you use an hp motherboard, you also have to enable unblockfsconnect in [UEFI-Quirks](https://dortania.github.io/OpenCore-Install-Guide/config-laptop.plist/ivy-bridge.html#quirks-4)

#### Haswell
- you have to specify your igpu in [DeviceProperties-Add](https://dortania.github.io/OpenCore-Install-Guide/config-laptop.plist/haswell.html#add-2)
- if you have missing bios options you have to edit [kernel-quirks](https://dortania.github.io/OpenCore-Install-Guide/config-laptop.plist/haswell.html#quirks-3)
    - if you have an hp laptop you may enable LapicKernelPanic
- to change bootargs edit [NVRAM-Add](https://dortania.github.io/OpenCore-Install-Guide/config-laptop.plist/haswell.html#add-4)
- if your device has no Native support for nvram you should edit [NVRAM-Delete](https://dortania.github.io/OpenCore-Install-Guide/config-laptop.plist/haswell.html#delete-3)
- you have to change the SMBios, and add all the missing info(mlb,rom,product,serial) in [Platforminfo](https://dortania.github.io/OpenCore-Install-Guide/config-laptop.plist/haswell.html#platforminfo)
- if you use an hp motherboard, you also have to enable unblockfsconnect in [UEFI-Quirks](https://dortania.github.io/OpenCore-Install-Guide/config-laptop.plist/haswell.html#quirks-4)

#### Broadwell
- if you have an hd5600 [DeviceProperties-Add](https://dortania.github.io/OpenCore-Install-Guide/config-laptop.plist/broadwell.html#add-2)
    - also if you have a kernel panic you have to add some additional properties.
- if you have missing bios options you have to edit [kernel-quirks](https://dortania.github.io/OpenCore-Install-Guide/config-laptop.plist/broadwell.html#quirks-3)
    - if you have an hp laptop you may enable LapicKernelPanic
- to change bootargs edit [NVRAM-Add](https://dortania.github.io/OpenCore-Install-Guide/config-laptop.plist/broadwell.html#add-4)
- if your device has no Native support for nvram you should edit [NVRAM-Delete](https://dortania.github.io/OpenCore-Install-Guide/config-laptop.plist/broadwell.html#delete-3)
- you have to change the SMBios, and add all the missing info(mlb,rom,product,serial) in [Platforminfo](https://dortania.github.io/OpenCore-Install-Guide/config-laptop.plist/broadwell.html#platforminfo)
- if you use an hp motherboard, you also have to enable unblockfsconnect in [UEFI-Quirks](https://dortania.github.io/OpenCore-Install-Guide/config-laptop.plist/broadwell.html#quirks-4)

- **Dell users:**
**skylake and newer**
    - Kernel -> Quirk -> CustomSMBIOSGuid -> True
    - PlatformInfo -> UpdateSMBIOSMode -> Custom


#### Skylake
- specify what gpu you have in APPL,ig-platform-id inside[DeviceProperties-Add](https://dortania.github.io/OpenCore-Install-Guide/config-laptop.plist/skylake.html#add-2)
    - if you have an hd510 gpu you may add more properties.
- if you have missing bios options you have to edit [kernel-quirks](https://dortania.github.io/OpenCore-Install-Guide/config-laptop.plist/skylake.html#quirks-3)
    - if you have an hp laptop you may enable LapicKernelPanic
- to change bootargs edit [NVRAM-Add](https://dortania.github.io/OpenCore-Install-Guide/config-laptop.plist/skylake.html#add-4)
- if your device has no Native support for nvram you should edit [NVRAM-Delete](https://dortania.github.io/OpenCore-Install-Guide/config-laptop.plist/skylake.html#delete-3)
- you have to change the SMBios, and add all the missing info(mlb,rom,product,serial) in [Platforminfo](https://dortania.github.io/OpenCore-Install-Guide/config-laptop.plist/skylake.html#platforminfo)
- if you use an hp motherboard, you also have to enable unblockfsconnect in [UEFI-Quirks](https://dortania.github.io/OpenCore-Install-Guide/config-laptop.plist/skylake.html#quirks-4)

#### Kaby Lake
- specify what gpu you have in APPL,ig-platform-id inside[DeviceProperties-Add](https://dortania.github.io/OpenCore-Install-Guide/config-laptop.plist/kaby-lake.html#add-2)
- if you have missing bios options you have to edit [kernel-quirks](https://dortania.github.io/OpenCore-Install-Guide/config-laptop.plist/kaby-lake.html#quirks-3)
    - if you have an hp laptop you may enable LapicKernelPanic
- to change bootargs edit [NVRAM-Add](https://dortania.github.io/OpenCore-Install-Guide/config-laptop.plist/kaby-lake.html#add-4)
- if your device has no Native support for nvram you should edit [NVRAM-Delete](https://dortania.github.io/OpenCore-Install-Guide/config-laptop.plist/kaby-lake.html#delete-3)
- you have to change the SMBios, and add all the missing info(mlb,rom,product,serial) in [Platforminfo](https://dortania.github.io/OpenCore-Install-Guide/config-laptop.plist/kaby-lake.html#platforminfo)
- if you use an hp motherboard, you also have to enable unblockfsconnect in [UEFI-Quirks](https://dortania.github.io/OpenCore-Install-Guide/config-laptop.plist/kaby-lake.html#quirks-4)

#### Coffee Lake
- specify what gpu you have in APPL,ig-platform-id inside[DeviceProperties-Add](https://dortania.github.io/OpenCore-Install-Guide/config-laptop.plist/coffee-lake.html#add-2)
- if you have missing bios options you have to edit [kernel-quirks](https://dortania.github.io/OpenCore-Install-Guide/config-laptop.plist/coffee-lake.html#quirks-3)
    - if you have an hp laptop you may enable LapicKernelPanic
- to change bootargs edit [NVRAM-Add](https://dortania.github.io/OpenCore-Install-Guide/config-laptop.plist/coffee-lake.html#add-4)
- if your device has no Native support for nvram you should edit [NVRAM-Delete](https://dortania.github.io/OpenCore-Install-Guide/config-laptop.plist/coffee-lake.html#delete-3)
- you have to change the SMBios, and add all the missing info(mlb,rom,product,serial) in [Platforminfo](https://dortania.github.io/OpenCore-Install-Guide/config-laptop.plist/coffee-lake.html#platforminfo)
- if you use an hp motherboard, you also have to enable unblockfsconnect in [UEFI-Quirks](https://dortania.github.io/OpenCore-Install-Guide/config-laptop.plist/coffee-lake.html#quirks-4)


#### Coffee Lake Plus
- specify what gpu you have in APPL,ig-platform-id inside[DeviceProperties-Add](https://dortania.github.io/OpenCore-Install-Guide/config-laptop.plist/coffee-lake-plus.html#add-2)
- if you have missing bios options you have to edit [kernel-quirks](https://dortania.github.io/OpenCore-Install-Guide/config-laptop.plist/coffee-lake-plus.html#quirks-3)
    - if you have an hp laptop you may enable LapicKernelPanic
- to change bootargs edit [NVRAM-Add](https://dortania.github.io/OpenCore-Install-Guide/config-laptop.plist/coffee-lake-plus.html#add-4)
- if your device has no Native support for nvram you should edit [NVRAM-Delete](https://dortania.github.io/OpenCore-Install-Guide/config-laptop.plist/coffee-lake-plus.html#delete-3)
- you have to change the SMBios, and add all the missing info(mlb,rom,product,serial) in [Platforminfo](https://dortania.github.io/OpenCore-Install-Guide/config-laptop.plist/coffee-lake-plus.html#platforminfo)
- if you use an hp motherboard, you also have to enable unblockfsconnect in [UEFI-Quirks](https://dortania.github.io/OpenCore-Install-Guide/config-laptop.plist/coffee-lake-plus.html#quirks-4)


#### Ice Lake
- if you cant set the DVMT-prealloc of your igpu you have to add additional values inside[DeviceProperties-Add](https://dortania.github.io/OpenCore-Install-Guide/config-laptop.plist/icelake.html#add-2)
- if you have missing bios options you have to edit [kernel-quirks](https://dortania.github.io/OpenCore-Install-Guide/config-laptop.plist/icelake.html#quirks-3)
    - if you have an hp laptop you may enable LapicKernelPanic
- to change bootargs edit [NVRAM-Add](https://dortania.github.io/OpenCore-Install-Guide/config-laptop.plist/icelake.html#add-4)
- if your device has no Native support for nvram you should edit [NVRAM-Delete](https://dortania.github.io/OpenCore-Install-Guide/config-laptop.plist/icelake.html#delete-3)
- you have to change the SMBios, and add all the missing info(mlb,rom,product,serial) in [Platforminfo](https://dortania.github.io/OpenCore-Install-Guide/config-laptop.plist/icelake.html#platforminfo)
- if you use an hp motherboard, you also have to enable unblockfsconnect in [UEFI-Quirks](https://dortania.github.io/OpenCore-Install-Guide/config-laptop.plist/icelake.html#quirks-4)