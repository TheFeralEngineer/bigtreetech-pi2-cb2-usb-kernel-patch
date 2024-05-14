# bigtreetech-pi2-cb2-usb-kernel-patch
enable all USB drivers on BTT Pi2 and CB2 to work on various 3D printer boards and devices. <br >
For some reason, Bigtreetech did not enable critical drivers such as the ch341 driver on their newest Klipper boards, rendering them pretty useless for the time being. <br >
As a workaround, you can use GPIO pins 21 and 23 along with a serial UART communication interface by enabling uart5 in armbianBoardEnv.txt (with a properly compiled binary, of course ;] ), but here is a fix if you wish to use USB<br >
 <br > <br >
To use this file: <br >
Copy the .tar file to your CB2 using WinSCP
<br ><br >
SSH into the CB2/Pi2 and navigate to the folder where you copied the tar file to. <br >
`cd ./{kernel-patch-folder}`

Extract the .tar file:<br >
`tar -xvf kernel-bigtree-cb2-legacy*.tar`

You should get two .deb files. <br > <br >
Install the new kernel on the CB2: <br >
`sudo dpkg -i *.deb`
 <br > <br >
Reboot: <br >
`sudo reboot now`
