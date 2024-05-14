# bigtreetech-pi2-cb2-usb-kernel-path
enable all USB drivers to work on various 3D printer boards and devices

To use this file:
Copy the .tar file to your CB2 using WinSCP

SSH into the CB2/Pi2 and navigate to the folder where you copied them to.
cd ./{kernel-patch-folder}

Extract the .tar file:
tar -xvf kernel-bigtree-cb2-legacy*.tar

You should get two .deb files. Install the new kernel on the CB2:
sudo dpkg -i *.deb

Reboot:
reboot
