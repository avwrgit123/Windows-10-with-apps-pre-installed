Windows-10-with-apps-pre-installed
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <!-- <title>Document</title> -->
</head>
<body>
<p>In this guide we install windows 10 with apps pre installed of your choose</p>
<p>*note after this guide you create a custom windows 10 contain on version apps your choose with to install.</p>
<p>This guide was inspired by video: https://www.youtube.com/watch?v=81yIxQ1RdiM</p>
<p>We use virtual machine in this guide</p>
<p>Check that virtualization is enabled in the bios on your computer <a href="https://www.isumsoft.com/computer-tweaks/enable-virtualization-technology-vt-x-in-bios-or-uefi.html">enabled virtualization on bios</a></p>
<a href="https://www.technewstoday.com/how-to-enable-virtualization-in-bios/">Check enabled virtualization on bios</a>
<h2>Software you need</h2>
<h2>Download according to you'r pc and os</h2>
<h2>virtual machine</h2>
<p>virtualbox <a href="https://www.oracle.com/virtualization/technologies/vm/downloads/virtualbox-downloads.html">virtualbox</a></p>
 <p>vmware <a href="https://knowledge.broadcom.com/external/article/309355/downloading-and-installing-vmware-workst.html">vmware</a></p>
<h2>windows 10</h2>
<p>windows 10 <a href="https://www.microsoft.com/en-us/software-download/windows10?msockid=017162c851b66f9e00e271f850266e87">windows 10</a></p>
<h2>windows pe</h2>
<p>hirens boot cd <a href="https://www.hirensbootcd.org/download/">hirens boot cd</a></p>
<p>WinPE10 8 Sergei Strelec <a href="https://sergeistrelec.name/winpe-10-8-sergei-strelec-english/241-winpe-11-10-8-sergei-strelec-x86x64native-x86-20240920-english-version.html">WinPE10 8 Sergei Strelec</a></p>
<h2>Capture windows with apps image</h2>
<p>Gimagex <a href="https://gimagex.software.informer.com/2.0/">Gimagex</a></p>
<p>ImageX <a href="https://wimlib.net/downloads/index.html">ImageX</a></p>
<p>Dism use command: dism.exe /capture-image /ImageFile:"D:\install.wim" /CaptureDir:C:\ /Name:win10apps /compress:max</p>
<p>Using dism command guide youtube: https://www.youtube.com/watch?v=-tIO4B8q8sk</p>
<h2>Edit iso</h2>
<p>Imgburn  <a href="https://www.imgburn.com/index.php?act=download">Imgburn</a></p>
<p>Poweriso <a href="https://www.poweriso.com/download.htm">poweriso</a></p>
<h2>Extract</h2>
<p>7zip <a href="https://www.7-zip.org/download.html">7zip</a></p>
<p>winrar <a href="https://www.win-rar.com/download.html?&L=0">winrar</a></p>
 
<p>I using virtualbox, windows 10 x64, hirens boot cd, Gimagex, Imgburn</p>
<p>I want to install winrar 7zip office for example</p>
<p>This guide create custom windows 10 on windows os</p>
<p>1. Download and Install virtualbox and Imgburn on your pc</p>
<p>2. Download Gimagex and windows 10 iso</p>
<p>Extract Gimagex put the exe file in usb using 7zip or winrar</p>

<h3>How to download windows 10 iso</h3>
<p>Press downloads on Create Windows 10 installation media it download MediaCreationTool.exe</p>
<img src="./pictures/Windows 10 installation media download.PNG">
<img src="./pictures/MediaCreationTool.PNG">
<p>press on MediaCreationTool.exe 2 times to start the program</p>
<p>accept the license agreement: press accept</p>
<p>after this wait a bit then choose from the options present to you the option "Create installation media (USB flash drive, DVD, or ISO) for another PC" then click "next"</p>
<img src="./pictures/‏‏windows 10 setup what to do.PNG">
<p>in the next window Select the language, architecture (x32/x64/both), and edition of Windows, you want then click "next" then click "ok"</p>
<img src="./pictures/‏‏‏‏windows 10 setup Select the language, architecture edition.PNG">
<p>in the next window Select ISO file give it a name and a path/location (where to save it) then click "next"</p>
<img src="./pictures/windows 10 setup Choose wich media to use.PNG">
<img src="./pictures/‏‏windows 10 setup choose where to save.PNG">
<p>then the tool will create your ISO file for you</p>
<p>when it finish click finish and it close the MediaCreationTool.exe</p>
<p>guide: <a href="https://support.microsoft.com/en-us/windows/create-an-iso-file-for-windows-10-38547366-1dcb-7afd-1726-9eb222d72705">guide</a></p>
<p>when the creation of windows iso is finish you see a windows.iso file in the location you choose</p>
<p>3. Create a virtual machine</p>
<h2>create a virtual machine</h2>
<p>start virtual box 2 clicks on virualbox shortcut</p>
<img src="./pictures/‏‏virtual box home screen.PNG">
<p>press new it create new machine</p>
<img src="./pictures/‏‏virtual box press new.PNG">
<p>in the windows that open give name to the machine,
choose were to save it-live it on default on windows is usely on C:\Users\your user\VirtualBox VMs,
don't select iso file we do this later
choose a type:windows
in the version choose windows 10 then click next</p>
<img src="https://github.com/avwrgit123/Windows-10-with-apps-pre-installed/blob/main/pictures/%E2%80%8F%E2%80%8F%E2%80%8F%E2%80%8Fvirtual%20box%20give%20name%20to%20machine.PNG">
<p>in the windows that open choose amount of ram to machine and amount of cpu to machine then click next</p>
<img src="./pictures/‏‏virtual box amount of ram and amount of cpu.PNG">
<p>in the windows that open choose amount of hdd to machine then click next</p>
<p>don't click on "pre allocate full size"-if you do it it take the amount from you'r physical hdd</p>
<img src="./pictures/‏‏virtual box amount of hdd.PNG">
<p>now the machine is created</p>
<p>you can edit the machine: right click on the mouse and choose setting beteen the options, cleeck on setting</p>
<img src="https://github.com/avwrgit123/Windows-10-with-apps-pre-installed/blob/main/pictures/%E2%80%8F%E2%80%8Fvirtual%20box%20machine%20setting.PNG">
<p>in setting go to boot make shoore on boot options "optical" and "hard disk" options are marked</p>
<p>move choose optical and move it above hard disk using the arrows then press "ok"</p>
<p>boot options tell the machine the order of boot sequence</p>
<p>optical option boot the machine from cd or iso</p>
<p>hard disk option boot the machine from hard disk</p>
<img src="https://github.com/avwrgit123/Windows-10-with-apps-pre-installed/blob/main/pictures/%E2%80%8F%E2%80%8Fvirtual%20box%20boot%20order%E2%80%8F%E2%80%8F.PNG">
<p>then go to storage</p>
<p>click on the blue disk name empty then click the blue disk from the right</p>
<p>then choose option 2 "choose from a disk file" from the options menu go to the location of windows iso and choose windows iso and fress "ok"</p>
<img src="https://github.com/avwrgit123/Windows-10-with-apps-pre-installed/blob/main/pictures/%E2%80%8F%E2%80%8F%E2%80%8F%E2%80%8Fvirtual%20box%20choose%20from%20a%20disk%20file%20option.PNG">
<p>now the blue disk name change from empty to windows.iso</p>
<p>then press "ok" on button of the setting menu -it save you'r changes and exit the setting menu</p>
<p>4. Install windows 10 on virtual box machine</p>
<h2>install windows 10 on virtual box machine</h2>
<p>on the main menu click 2 times on the machine or click 1 times on the machine and click start</p>
<img src="https://github.com/avwrgit123/Windows-10-with-apps-pre-installed/blob/main/pictures/%E2%80%8F%E2%80%8F%E2%80%8F%E2%80%8Fvirtual%20box%20start%20the%20machine.PNG">
<p>the installation program start choose your installation language, time zone, keyboard language then click "next"</p>
<img src="https://github.com/avwrgit123/Windows-10-with-apps-pre-installed/blob/main/pictures/%E2%80%8F%E2%80%8Fwindows%2010%20configre%20install.PNG">
<p>after this on the windows that open click the Install now button</p>
<img src="https://github.com/avwrgit123/Windows-10-with-apps-pre-installed/blob/main/pictures/windows%2010%20install%20now.PNG">
<p>after this this on the windows that open you will be prompted to enter the Windows 10 Product Key</p>
<p>you can click on the option that says I don’t have a product key and skip entering product key</p>
<img src="https://github.com/avwrgit123/Windows-10-with-apps-pre-installed/blob/main/pictures/%E2%80%8F%E2%80%8Fwindows%2010%20produck%20key.PNG">
<p>after this on the windows that open choose a version to install</p>
<p>i choose windows 10 pro then click "next"</p>
<img src="https://github.com/avwrgit123/Windows-10-with-apps-pre-installed/blob/main/pictures/%E2%80%8F%E2%80%8Fwindows%2010%20choos%20version%20to%20install.PNG">
<p>after this on the windows that open accept terms of use mark the option "i accept the license terms" then click "next"</p>
<img src="https://github.com/avwrgit123/Windows-10-with-apps-pre-installed/blob/main/pictures/%E2%80%8F%E2%80%8Fwindows%2010%20terms%20of%20use%20accept.PNG">
<p>after this on the windows that open click on custom install</p>
<p>update this option upgrade a working windows 10 when it run to ths version</p>
<p>custom install this option install fresh windows on the hard drive</p>
<img src="https://github.com/avwrgit123/Windows-10-with-apps-pre-installed/blob/main/pictures/%E2%80%8F%E2%80%8Fwindows%2010%20custom%20install.PNG">
<p>after this on the windows that open choose the hdd to install windows 10 on it then click "next"</p>
<img src="https://github.com/avwrgit123/Windows-10-with-apps-pre-installed/blob/main/pictures/%E2%80%8F%E2%80%8Fwindows%2010%20choose%20a%20hdd.PNG">
<p>after this on the windows that open windows 10 start to install on the hard drive"</p>
<img src="https://github.com/avwrgit123/Windows-10-with-apps-pre-installed/blob/main/pictures/%E2%80%8F%E2%80%8Fwindows%2010%20installing%20on%20hdd.PNG">
<p>when the installation is over the pc automatically restart</p>
<img src="https://github.com/avwrgit123/Windows-10-with-apps-pre-installed/blob/main/pictures/%E2%80%8F%E2%80%8Fwindows%2010%20option%20to%20restart%20after%20installing.PNG">
<p>now you get a screens to configure the region, keyboard layout and more</p>
<p>guide <a href="https://techwiser.com/how-to-install-windows-10-in-virtualbox/">guide</a></p>
<p>5. enter default administrator account before create a user</p>
<p>now press ctrl+shift+f3 keys together it enter you to a default administrator account in pre install system- oobe</p>
<img src="https://github.com/avwrgit123/Windows-10-with-apps-pre-installed/blob/main/pictures/%E2%80%8F%E2%80%8Fctrl%2Bshift%2Bf3%20keys.PNG">
<img src="https://github.com/avwrgit123/Windows-10-with-apps-pre-installed/blob/main/pictures/%E2%80%8F%E2%80%8Fwindows%2010%20default%20administrator%20account.PNG">
<p>on administrator account you install the softwares you want</p>
<p>6. install softwares on windows 10</p>
<p>now i show you the control panel before i install any softwares</p>
<p>search control panel on the search bar and click control panel it open a window called control pannell</p>
<p>on control panel you see programs and under it you see uninstall a program click on "uninstall a program"</p>
<img src="https://github.com/avwrgit123/Windows-10-with-apps-pre-installed/blob/main/pictures/%E2%80%8F%E2%80%8Fcontrol%20panel%20befor%20i%20install%20any%20softwares.PNG">
<p>i install some softwares and show you the control panel after i install any softwares</p>
<img src="https://github.com/avwrgit123/Windows-10-with-apps-pre-installed/blob/main/pictures/%E2%80%8F%E2%80%8Fcontrol%20panel%20after%20i%20install%20softwares.PNG">
<p>7. exit default administrator account using system preparation tool</p>
<p>now press on the window system preparation tool on "ok" the windows restart to before you enter default administrator account</p>
<p>what is system preparation tool? explaine in this article https://learn.microsoft.com/en-us/windows-hardware/manufacture/desktop/sysprep--generalize--a-windows-installation?view=windows-11</p>
<p>the system preparation tool is usuly in location: C:/windows/system32/sysprep/sysprep.exe</p>
<img src="https://github.com/avwrgit123/Windows-10-with-apps-pre-installed/blob/main/pictures/%E2%80%8F%E2%80%8Fsystem%20preparation%20tool.PNG">
<p>8. after this turn off the machine</p>
<p>now turn off the machine press x in the windows of the machine then open a menu mark "power off the machine" and press "ok"</p>
<img src="https://github.com/avwrgit123/Windows-10-with-apps-pre-installed/blob/main/pictures/%E2%80%8F%E2%80%8Fpower%20off%20windows%2010%20machine.PNG">
<p>9. let's add another hdd to the machine</p>
<h2>add another hdd to the machine</h2>
<p>do this when the machine is off</p>
<p>go to setting of the machine to storage press right click on the mouse on "controller: sata" choose hard disk then press left click on the mouse</p>
<img src="https://github.com/avwrgit123/Windows-10-with-apps-pre-installed/blob/main/pictures/controller%20sata%20choose%20hard%20disk.PNG">
<p>choose create new hdd and press "next"</p>
<img src="https://github.com/avwrgit123/Windows-10-with-apps-pre-installed/blob/main/pictures/create%20new%20hdd.PNG">
<p>choose vdi between the options</p>
<img src="https://github.com/avwrgit123/Windows-10-with-apps-pre-installed/blob/main/pictures/vdi%20hdd.PNG">
<p>give it a size and press "ok"</p>
<p>choose witch hdd to attach to machine mark it and press choose</p>
<img src="https://github.com/avwrgit123/Windows-10-with-apps-pre-installed/blob/main/pictures/choose%20new%20hdd%20to%20machine.PNG">
<p>inside storage you see the new hdd you created</p>
<img src="https://github.com/avwrgit123/Windows-10-with-apps-pre-installed/blob/main/pictures/add%20hdd%20success.PNG">
<p>press "ok" in buton of the setting menu to save you'r changes</p>
<p>10. add windows pe that you download to the cd choose the location the file located</p>
<p>the windows pe i download called HBCD_PE_x64.iso</p>
<p>yours may be different</p>
<p>11. run the machine</p>
<p>12. you see on the screen a massage: press any key to boot from cd or dvd</p>
<p>it appears for a few seconds</p>
<p>press any key on the keyboard</p>
<img src="https://github.com/avwrgit123/Windows-10-with-apps-pre-installed/blob/main/pictures/press%20any%20key%20to%20boot%20from%20cd%20or%20dvd%20massage.PNG">
<img src="https://github.com/avwrgit123/Windows-10-with-apps-pre-installed/blob/main/pictures/press%20any%20key%20to%20boot%20from%20cd%20or%20dvd%20massage2.PNG">
<p>it enter windows pe iso</p>
<p>13. extract Gimagex according to your windows version copy it to a usb</p>
<p>14. connect the usb to the machine</p>
<p>on the up of the machine window you see device press on it press usb and press on your usb</p>
<img src="https://github.com/avwrgit123/Windows-10-with-apps-pre-installed/blob/main/pictures/add%20usb%20hdd%20to%20machine.PNG">
<p>copy the Gimagex from the usb to windows pe</p>
<p>i copy Gimagex to desktop</p>
<p>15. let's copy Gimagex to the new hdd we created</p>
<h2>copy Gimagex to the new hdd we created</h2>
<p>remmber the new hdd we createt not active it not show up on windows pe</p>
<p>to active it press start (windows symbol) stand on this pc with the mouse press right click on the mouse press left on the mouse and on manage</p>
<img src="https://github.com/avwrgit123/Windows-10-with-apps-pre-installed/blob/main/pictures/this%20pc%20manage.PNG">
<p>from thier let's press disk management</p>
<img src="https://github.com/avwrgit123/Windows-10-with-apps-pre-installed/blob/main/pictures/press%20disk%20management.PNG">
<p>open a window ask you to configare the disk to mbr or gpt and press "ok"</p>
<p>it depend of your bios what it support</p>
<img src ="https://github.com/avwrgit123/Windows-10-with-apps-pre-installed/blob/main/pictures/disk%20configoration%20mbr%20or%20gpt.PNG">
<p>i choose gpt</p>
<img src ="https://github.com/avwrgit123/Windows-10-with-apps-pre-installed/blob/main/pictures/disk%20configoration%20choose%20gpt.PNG">
<p>now i see 2 colors: blue active black not active</p>
<p>color blue windows know this hdd exist</p>
<p>color black windows don't know this hdd exist</p>
<img src="https://github.com/avwrgit123/Windows-10-with-apps-pre-installed/blob/main/pictures/disk%20active%20or%20not%20active.PNG">
<p>now let's go to the unactive hdd-its the new hdd we created</p>
<p>stand on it press right click on the mouse a menu open up</p>
<p>press "new simple volume"</p>
<img src="https://github.com/avwrgit123/Windows-10-with-apps-pre-installed/blob/main/pictures/new%20simple%20volume.PNG">
<p>a menu open up give it the default press "next" and to start the proses on the last windows press "finish"</p>
<p>if the proses succseed you see the hdd color change to blue</p>
<img src="https://github.com/avwrgit123/Windows-10-with-apps-pre-installed/blob/main/pictures/after%20active%20the%20hdd%20success.PNG">
<p>you can exit disk management</p>
<p>i copy Gimagex to the new hdd we created</p>
<p>16. 2 click on Gimagex.exe</p>
<p>now open a window</p>
<h2>use Gimagex to capture windows 10 files</h2>
<p>You create file.wim in windows it called install.wim</p>
<p>i create the capture file in the second hdd we created</p>
<p>install.wim vs install.esd explained</p>
<p>https://www.reddit.com/r/windows/comments/gtcdci/whats_the_difference_between_esd_and_wim_and/?rdt=51366</p>
<p>https://windowsreport.com/convert-windows-11-install-wim-to-install-esd/#:~:text=The%20ESD%20%28Electronic%20Software%20Download%29%20file%20format%20uses,meaning%20you%20can%20update%2C%20add%2C%20or%20remove%20components.</p>
<p>on capture tag choose a source click browse choose what hdd you want to capture</p>
<p>on capture tag choose a destination click browse choose where to save the capture file and give it a name</p>
<p>capture file extension is .wim</p>
<p>on capture tag in the option tag mark boot, verify</p>
<p>then click on create batton - it create the file.wim</p>
<img src="https://github.com/avwrgit123/Windows-10-with-apps-pre-installed/blob/main/pictures/use%20Gimagex%20software.PNG">
<img src="https://github.com/avwrgit123/Windows-10-with-apps-pre-installed/blob/main/pictures/Gimagex%20capture%20prosses%20start.PNG">
<p>if you want to cancel the catpure click abort batton</p>
<p>when the prosses is finish click close batton</p>
<img src="https://github.com/avwrgit123/Windows-10-with-apps-pre-installed/blob/main/pictures/Gimagex%20capture%20prosses%20finish.PNG">
<p>exit the Gimagex.exe</p>
<p>you can check see the file.wim</p>
<p>exit windows pe</p>
<p>copy the file.wim to you'r pc vie a usb</p>
<p>17. create new iso with apss</p>
<h2>create new iso with apss</h2>
<p>run imageburn click 2 times on imageburn</p>
<p></p>




</body>
</html>
