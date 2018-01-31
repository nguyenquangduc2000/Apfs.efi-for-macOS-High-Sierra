# Apfs.efi for macOS High Sierra

Ever since Apple introduced the new File system (Apple File System - a.k.a APFS) in macOS High Sierra, there’s a need to add an additional driver called apfs.efi into our Clover in order to boot successfully. Apfs.efi is installed in either /EFI/Clover/drivers64UEFI or /EFI/Clover/drivers64 folder depending on the bios system that we have (UEFI/Legacy). 

Like kexts, to stay updated, apfs.efi  should be updated concurrently with each new High Sierra release. The good news is that High Sierra, even the combo updates are shipped with apfs.efi driver in it under (/usr/standalone/i386/). You can always go-ahead  to use this apfs.efi as it is if you want. But, it has an annoying problem, at least for me.
The original apfs.efi extracted from /usr/standalone/i386/ displays some flash messages (verbose texts) when it is loaded. Usually, just before the Clover Menu. 

![d6e06de6a7cc965d0375214bd0137c7a](https://user-images.githubusercontent.com/23084817/35628629-7b799c24-06d7-11e8-9625-638d8a18735c.jpg)

For me, it is not aesthetically pleasing to see such messages on every reboot. Therefore, a patched apfs.efi was needed to hide those messages at boot up. Thus, this repository provides the modified apfs.efi versions for your convenience. 

Thank you.

macOS High Sierra 10.13.3

apfs.efi


