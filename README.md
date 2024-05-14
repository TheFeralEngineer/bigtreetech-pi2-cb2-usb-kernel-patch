# bigtreetech-pi2-cb2-usb-kernel-patch
enable all USB drivers to work on various 3D printer boards and devices
 <br > <br >
To use this file: <br >
Copy the .tar file to your CB2 using WinSCP
<br ><br >
SSH into the CB2/Pi2 and navigate to the folder where you copied them to. <br >
`cd ./{kernel-patch-folder}`

Extract the .tar file:<br >
`tar -xvf kernel-bigtree-cb2-legacy*.tar`

You should get two .deb files. <br > <br >
Install the new kernel on the CB2: <br >
`sudo dpkg -i *.deb`
 <br > <br >
Reboot: <br >
`sudo reboot now`
