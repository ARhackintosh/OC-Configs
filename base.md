# Base.plist settings
- add warnings
- remove acpi entries
## DeviceProperties --> ADD
- remove PciRoot(0x0)/Pci(0x1b,0x0)
- add PciRoot(0x0)/Pci(0x2,0x0)
- add AAPL,ig-platform-id under PciRoot(0x0)/Pci(0x2,0x0)
## Kernel
### Add
- remove all default kexts
### Quirks
- enable PanicNoKextDump
- enable PowerTimeoutKernelPanic
- enable XhciPortLimit
## misc
### Debug
- enable AppleDebug
- enable ApplePanic
- enable DisableWatchDog
- Target = 67
### Security
- enable AllowNvramReset
- enable AllowSetDefault
- enable BlacklistAppleUpdate
- ScanPolicy = 0
- SecureBootModel = Default
- Vault = Optional
## NVRAM
### 7C436110-AB2A-4BBB-A880-FE41995C9F82
- add debug=0x100
