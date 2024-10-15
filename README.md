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
<p>now press ctrl+shift+f3 keys together it enter you to a default administrator account in pre install system- oobe</p>
<img src="https://github.com/avwrgit123/Windows-10-with-apps-pre-installed/blob/main/pictures/%E2%80%8F%E2%80%8Fctrl%2Bshift%2Bf3%20keys.PNG">
<img src="https://github.com/avwrgit123/Windows-10-with-apps-pre-installed/blob/main/pictures/%E2%80%8F%E2%80%8Fwindows%2010%20default%20administrator%20account.PNG">
<p>on administrator account you install the softwares you want</p>
<p>now i show you the control panel before i install any softwares</p>
<p>search control panel on the search bar and click control panel it open a window called control pannell</p>
<p>on control panel you see programs and under it you see uninstall a program click on "uninstall a program"</p>
<img src="https://github.com/avwrgit123/Windows-10-with-apps-pre-installed/blob/main/pictures/%E2%80%8F%E2%80%8Fcontrol%20panel%20befor%20i%20install%20any%20softwares.PNG">
<p>i install some softwares and show you the control panel after i install any softwares</p>
<img src="https://github.com/avwrgit123/Windows-10-with-apps-pre-installed/blob/main/pictures/%E2%80%8F%E2%80%8Fcontrol%20panel%20after%20i%20install%20softwares.PNG">
<p>now press on the window system preparation tool on "ok" the windows restart to before you enter default administrator account</p>
<p>what is system preparation tool? explaine in this article https://learn.microsoft.com/en-us/windows-hardware/manufacture/desktop/sysprep--generalize--a-windows-installation?view=windows-11</p>
<p>the system preparation tool is usuly in location: C:/windows/system32/sysprep/sysprep.exe</p>
<img src="https://github.com/avwrgit123/Windows-10-with-apps-pre-installed/blob/main/pictures/%E2%80%8F%E2%80%8Fsystem%20preparation%20tool.PNG">



<p></p>

</body>
</html>
