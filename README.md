# openCore-clover-arm64-psuedo-design
psuedo-design openCore-arm64


* transistion openCore to arm64 -> place a "bare" metal KVM/XEN style qemu-system-arm64 image into the boot area as a < 2GB loadable system-image to read from /dev/sda or /dev/sdb directly as a nested libvirtd function for boot wrapped into OpenCore to read :boot0 ,, booti386 , apfs.efi (not boot-132)

read qemu-system-arm64.img scan /dev/sda , /dev/sdb , /dev/sdc for boot area HFSplus.efi, ext4.efi, etc,

(ESXI style small boot area < 500MB) -> wrap KVM -> OpenCore arm64



macOS -next version as KVM/XEN bare metal OpenCore bootloader (amd64)
