# Update Thinkpad BIOS

1. Download the **BIOS Updatable Bootable CD** from [support.lenovo.com](https://support.lenovo.com)
2. Use [geteltorito](https://userpages.uni-koblenz.de/~krienke/ftp/noarch/geteltorito/) to extract a bootable image

```bash
geteltorito -o bios.img $LENOVO_BOOTABLE_CD.iso
```

3. Copy the image to USB drive

```bash
sudo dd if=bios.img of=/dev/$USB_FLASH_DRIVE
```

4. Synconize cached writes to persistent storage

```bash
sudo sync
```

## References

- [LENOVO BIOS/UEFI UPDATE FROM USB STICK (WITHOUT BOOTABLE CD)](http://tojaj.com/lenovo-biosuefi-update-from-usb-stick-i-e-without-bootable-cd/)
