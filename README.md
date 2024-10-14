Windows-10-with-apps-pre-installed
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
</head>
<body>
<p>In this guide we install windows 10 with apps pre installed of your choose</p>
<p>*note after this guide you create a custom windows 10 contain on version apps your choose with to install.</p>
<p>This guide was inspired by video: https://www.youtube.com/watch?v=81yIxQ1RdiM</p>
<p>We use virtual machine in this guide</p>
<p>Check that virtualization is enabled in the bios on your computer</p>
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
<p>guide: <a href="https://support.microsoft.com/en-us/windows/create-an-iso-file-for-windows-10-38547366-1dcb-7afd-1726-9eb222d72705">guide</a></p>
<p>when the creation of windows iso is finish you see a windows.iso file in the location you choose</p>
<h2>create a virtual machine</h2>
<p>start virtual box 2 clicks on virualbox shortcut</p>
<img src="./pictures/‏‏virtual box home screen.PNG">
<p>press new it create new machine</p>
<img src="./pictures/‏‏virtual box press new.PNG"
<p>in the windows that open give name to the machine,
choose were to save it-live it on default on windows is usely on C:\Users\your user\VirtualBox VMs,
don't select iso file we do this later
choose a type:windows
in the version choose windows 10 then click next</p>
<img src="./pictures/‏‏virtual box give name to machine.PNG"
<p>in the windows that open choose amount of ram to machine and amount of cpu to machine then click next</p>
<img src="./pictures/‏‏virtual box amount of ram and amount of cpu.PNG"
<p>in the windows that open choose amount of hdd to machine then click next</p>
<p>don't click on "pre allocate full size-if you do it it take the amount from you'r physical hdd"</p>
<img src="./pictures/‏‏virtual box amount of hdd.PNG"
    
</body>
</html>
