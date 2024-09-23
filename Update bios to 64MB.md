
# How to change bios to 64MB DVMT allocated VRAM

### WARNING ONLY DO THIS IF YOU HAVE A DELL LATITUDE 5290!!

### Failure to do so may brick your laptop!!!

Start by downloading the [EFI Shell](https://github.com/lukeshondas/Dell-Latitude-5290-Opencore/blob/main/EFI%20Shell.zip), extract the zip and copy the boot folder inside your EFI folder on a fat32 partition or USB.

Once booted into the shell type `setup_var 0x804 0x2` then type `reboot` and your laptop will be all set for higher resoultion monitors and better gpu performance.

You can now use the EFI without the Framebuffer patch.