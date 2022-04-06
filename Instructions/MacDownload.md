<a href="../Home/index.html" class="btn">Home</a> <a href="Releases.html" class="btn">Downloads</a> <a href="../Contact/contact.html" class="btn">Contact</a> <a href="WindowsDownload.html" class="btn">Windows Install</a> <a href="../Instructions/MacDownload.html" class="btn">MacOS Install</a> <a href="https://github.com/kelpup/woof-CE" class="btn">Contribute</a> <a href="../User/user.html" class="btn">User Help</a> 

# MacOS Instructions for Running Kelpup

### What You'll Need
```markdown
- A 1 GB or larger flashdrive
- Wifi
- A laptop running MacOS
- Time!
```

### Note for M1 Users
There's a chance that disabling secure boot doesn't work on your Mac- you might have an M1 chip, or a newer Intel chip that has SIP (system integrity protection). If that's the case, you can run a virtual machine using Virtual Box instead! Here is a good <a href="https://ubuntu.com/tutorials/how-to-run-ubuntu-desktop-on-a-virtual-machine-using-virtualbox#1-overview" style="color: #b5e853; text-decoration: underline;text-decoration-style: dotted;">tutorial</a> on how to make a virtual machine on Virtual Box with Ubuntu. Just follow these directions are replace the Ubuntu ISO with the Kelpup ISO you downloaded.

What's an M1? It's a "System on a Chip" that's a CPU and a GPU (central processing unit and a graphics processing unit). Basically, the heart of your laptop. Some Macs have Intel chips, and some Macs have Apple-made M1 chips. Here's an <a href="https://www.laptopmag.com/news/apple-m1-vs-intel-cpu-this-is-the-best-processor-for-your-laptop" style="color: #b5e853; text-decoration: underline;text-decoration-style: dotted;">article</a> about the difference.

### Step 1 - Download ISO
We say that you can "burn our ISO" onto a flashdrive, and use that to run our disro on your computer. But what does that really mean? 

> "The idea behind an ISO imge is that you can archive an exact digital copy of a disc, and then later use that image to burn a new disc that's in turn an exact copy of the original (...) most operating systems allow you to mount an ISO image as a virtual disc, in which case all your apps treat it as if a real optical disc were inserted." - (<a href="https://www.howtogeek.com/356714/what-is-an-iso-file-and-how-do-i-open-one/" style="color: #b5e853; text-decoration: underline;text-decoration-style: dotted;">source</a>)

So when you download our ISO file, it is really just a copy of the linux distribution we have created. By "burning" it onto a flashdrive, you are just making your own portable copy that you can then insert and boot on your own machine.

Download the lastest release from the <a href="Releases.html" style="color: #b5e853; text-decoration: underline;text-decoration-style: dotted;">Downloads</a> page, but don't open it! It's an ISO- it's not meant to be opened like a folder or a file.

### Step 2 - Format USB
1) Open Finder, and select the Applications tab from the lefthand side. Then, click on the Utilities foler. 

<img width="115" alt="Screen_Shot_2022-02-21_at_10 41 53_PM" src="https://user-images.githubusercontent.com/65368903/155399733-d08c9905-aa7d-42fe-99d9-4b9870aaff28.png">

2) Click on the Disk Utility application.

<img width="101" alt="Screen_Shot_2022-02-21_at_10 42 10_PM" src="https://user-images.githubusercontent.com/65368903/155399816-1ee4bf06-8504-479c-b9d1-48ec9baab9a5.png">

3) The Disk Utility application will show you all of the disks that your laptop has access to. The internal ones are the drives actually inside your computer, and the external drives are things like USBs and other things you physically plug into your laptop. Disk images can be ignored. Plug in your USB to one of the ports of your laptop, and you should see it appear under External. Select it.

![Screen_Shot_2022-02-21_at_10 44 15_PM](https://user-images.githubusercontent.com/65368903/155399927-b2f7a270-93ce-4c0f-b666-a54091896f97.png)

Note: If your USB does not appear under External when you plug it in, it might be formatted in a way that your computer doesn't understand. Just try another USB.

4) From the top right, select Erase. Rename your USB to whatever you want, and select MS-DOS (FAT) as the format. 

![Screen_Shot_2022-02-21_at_10 44 56_PM](https://user-images.githubusercontent.com/65368903/155400385-4f0f20a1-2858-4e15-b62c-0b81304f224d.png)

Note: If there's also Scheme option for your USB, set it as GUID Partition Map.

5) Hit Erase, and wait for the program to finish running. Now your USB is properly formatted! Don't worry if your computer sends you a message saying it can't read it- we formatted it to be bootable from, so it's not sure what to do with the USB at this point. We'll fix it in the next section!

### Step 3 - Burn ISO to USB
1) Download <a href="https://unetbootin.github.io/" style="color: #b5e853; text-decoration: underline;text-decoration-style: dotted;">UNetbootin</a>.
2) Open your Downloads folder, and double click on unetbootin.dmg.
3) Double click on the UNetbootin application.

![Screen_Shot_2022-02-21_at_10 35 03_PM](https://user-images.githubusercontent.com/65368903/155394722-f4610b68-ae11-4a1f-9c14-539289364ae4.png)

Note: At this point, it will likely not open, as the application is from an unidentified developer. If it does open, skip to step 8. If it does not open, follow these next steps.
4) Open System Preferences by clicking on the apple icon on the top left and selecting System Preferences. Once it's open, click on Security & Privacy. Then, click on the General tab. Click on the little padlock icon on the bottom left and enter your password to be able to make changes.

![Screen_Shot_2022-02-21_at_10 36 17_PM](https://user-images.githubusercontent.com/65368903/155395276-e2dd85cb-19c6-4e06-841c-ab478b48175c.png)

5) A message should pop up telling you that UNetbootin was prevented from running. Click the option to allow it to run. Ensure App Store and identified developers is checked under Allow apps downloaded from.
6) Double click the UNetbootin application again, and enter your password.

![Screen_Shot_2022-02-21_at_10 37 31_PM](https://user-images.githubusercontent.com/65368903/155395731-d83bb767-a24b-45b1-b3e3-7f76f49f8f1c.png)

Note: Your laptop protects your USBs from applications, so they can't make changes like deleting your files behind your back. However, since we want to install KelPup to the USB, you'll have to give UNetbootin permission to do so, which is why it asks for your password.
Note: UNetbootin will ask for your password every time you open it- it can't access your USBs after you close it. Don't worry- it's not gonna overwrite anything behind your back.

7) When UNetbootin opens, select ISO in in the middle section, and click the button with the three dots on the righthand side and navigate to your downloaded KelPup ISO file. You might have to give UNetbootin permission to access your Downloads folder. It'll be called something like "kelpup62-x.x.iso" where x.x is the version you downloaded. Select it and hit open. Select USB Drive under the Type dropdown menu. 

![Screen_Shot_2022-02-21_at_10 38 31_PM](https://user-images.githubusercontent.com/65368903/155396157-3583d5c5-fa8b-45e5-97f6-5e403b22fd6c.png)

8) The Drive dropdown menu will list external drives (like USBs) plugged into your computer. If it's empty, that's okay. Plug in your USB, and restart UNetbootin, and a name should pop up (make sure to re-do the steps above!). It's good practice to unplug any other external drives (like other USBs) while you're doing this so you don't accidently overwrite them. The drive won't be named what your USB is named, but something similar to /dev/disk2s1. These names are what your laptop calls external USBs. 
Note: If you're concerned you don't have the right drive selected, unplug and restart UNetbootin. The USB should disapear from the drive options. You'll probably have to restart UNetbootin after plugging the USB back in.
Note: If you're USB STILL doesn't show up, it's probably just not formatted correctly. Go to the USB formatting instructions!
Note: You will probably have to hit okay to allow UNetbootin to access volumes on a usable volume

9) Hit Okay, and wait for the program to finish running. This might take a while- it is transferring an entire operating system onto your USB. Once it's done, you have a bootable USB! 

Note: DON'T take out your USB after this- we're gonna boot off of it!

### Step 4 - Disable Secure Boot to allow dual-booting off of a USB
Note: These steps are somewhat dangerous- if you mess around, you could end up factory resetting your laptop. But if you follow the instructions carefully, it'll be fine!

1) For these next steps, you'll have to reboot your computer, enter recovery mode, and disable secure boot, so you can't have these instructions pulled up at the same time. Probably best to take a photo or write down these instructions. 
2) Restart your Mac. When the Apple logo appears, hold "Command-R" to bring up the "macOS Recovery" menu. 
3) Select your language and hit the next arrow.
4) Click on the Utilities tab on the top left, and select Startup Security Utility, and enter your password when the account information pops up. It probably won't be an option on the middle box. 
5) On the Startup Security Utility screen, select "No Security" under Secure Boot and "Allow booting from external or removable media" under Allowed Boot Media.

![image-20181128060256-2](https://user-images.githubusercontent.com/65368903/160194400-a378f926-db58-473d-ab2f-37fe43116ca6.png)

6) Hit the red X button on the Startup Security Utility screen, then click the apple on the top left and select Restart. 
7) While the computer is restarting, HOLD DOWN the [option] key until your computer brings up the boot loader menu. Select your wifi and then click the non-MacOS option- it might be called Windows, but it's really Kelpup.
Note: If it doesn't work the first time and just brings up the MacOS, try, try again! Make sure to hold the [option] key down the entire time the computer is starting.

9) While Kelpup is booting, select the default first option for everything. Now you're running Kelpup!!

When you're done with Kelpup, just hit the power button and turn your computer off. Hit the power button again to turn it back on, and macOS will start automatically. You can save your session if you'd like, but if you got Kelpup to work, we think you should try your hand at a bunch of distros, and decide which one is your favorite! Kelpup isn't designed to be a home base distro, but a stepping stone. 

Look into booting Ubuntu off of a USB or dual-booting with Ubuntu by partitioning your drive :)

### Video Tutorial for Mac
[![Tutorial for Mac USB Formatting and ISO Burning](https://img.youtube.com/vi/afqgf71CjMQ/0.jpg)](https://www.youtube.com/watch?v=afqgf71CjMQ)

Click anywhere on the image

### What's Next? 
Now that you've successfully dual-booted your computer with a bootable USB running Kelpup, you could do the same process with almost any Linux distro!! 

A super functional distro you could use is <a href="https://ubuntu.com/tutorials/create-a-usb-stick-on-macos#1-overview" style="color: #b5e853; text-decoration: underline;text-decoration-style: dotted;">Ubuntu</a> - accessible, comes with a bunch of free applications, very user-friendly.

