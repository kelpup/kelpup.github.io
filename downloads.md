## Downloads Page!

SO, you want to dual-boot your laptop with Puppy Linux. Now what? You'll need a USB that doesn't have anything important on it, your laptop, and internet connection. 

### MacOS: Format USB to properly boot off of it
1. Open Finder, and select the Applications tab from the lefthand side. Then, click on the Utilities foler. 

<img width="115" alt="Screen_Shot_2022-02-21_at_10 41 53_PM" src="https://user-images.githubusercontent.com/65368903/155399733-d08c9905-aa7d-42fe-99d9-4b9870aaff28.png">

2. Click on the Disk Utility application.

<img width="101" alt="Screen_Shot_2022-02-21_at_10 42 10_PM" src="https://user-images.githubusercontent.com/65368903/155399816-1ee4bf06-8504-479c-b9d1-48ec9baab9a5.png">

3. The Disk Utility application will show you all of the disks that your laptop has access to. The internal ones are the drives actually inside your computer, and the external drives are things like USBs and other things you physically plug into your laptop. Disk images can be ignored. Plug in your USB to one of the ports of your laptop, and you should see it appear under External. Select it.

![Screen_Shot_2022-02-21_at_10 44 15_PM](https://user-images.githubusercontent.com/65368903/155399927-b2f7a270-93ce-4c0f-b666-a54091896f97.png)

Note: If your USB does not appear under External when you plug it in, it might be formatted in a way that your computer doesn't understand. Just try another USB.

4. From the top right, select Erase. Rename your USB to whatever you want, and select MS-DOS (FAT) as the format. 

![Screen_Shot_2022-02-21_at_10 44 56_PM](https://user-images.githubusercontent.com/65368903/155400385-4f0f20a1-2858-4e15-b62c-0b81304f224d.png)

Note: If there's also Scheme option for your USB, set is as GUID Partition Map.

5. Hit Erase, and wait for the program to finish running. Now your USB is properly formatted! Don't worry if your computer sends you a message saying it can't read it- we formatted it to be bootable from, so it's not sure what to do with the USB at this point. We'll fix it in the next section!

### MacOS: Create Bootable USB
1. Download [UNetbootin](https://unetbootin.github.io/).
2. Open your Downloads folder, and double click on unetbootin.dmg.
3. Double click on the UNetbootin application.

![Screen_Shot_2022-02-21_at_10 35 03_PM](https://user-images.githubusercontent.com/65368903/155394722-f4610b68-ae11-4a1f-9c14-539289364ae4.png)

Note: At this point, it will likely not open, as the application is from an unidentified developer. If it does open, skip to step 8. If it does not open, follow these next steps.
4. Open System Preferences, and click Security & Privacy. Click on the lock icon at the bottom right to enable changes. 

![Screen_Shot_2022-02-21_at_10 36 17_PM](https://user-images.githubusercontent.com/65368903/155395276-e2dd85cb-19c6-4e06-841c-ab478b48175c.png)

5. A message should pop up telling you that UNetbootin was prevented from running. Click the option to allow it to run. Ensure App Store and identified developers is checked under Allow apps downloaded from.
6. Double click the UNetbootin application again, and enter your password.

![Screen_Shot_2022-02-21_at_10 37 31_PM](https://user-images.githubusercontent.com/65368903/155395731-d83bb767-a24b-45b1-b3e3-7f76f49f8f1c.png)

Note: Your laptop protects your USBs from applications, so they can't make changes like deleting your files behind your back. However, since we want to install KelPup to the USB, you'll have to give UNetbootin permission to do so, which is why it asks for your password.
8. When UNetbootin opens, select PuppyLinux from the Distribution dropdown menu. Ensure ISO is selected in the middle section, and click the button with the three dots on the righthand side and navigate to your downloaded KelPup ISO file. Select USB Drive under the Type dropdown menu.

![Screen_Shot_2022-02-21_at_10 38 31_PM](https://user-images.githubusercontent.com/65368903/155396157-3583d5c5-fa8b-45e5-97f6-5e403b22fd6c.png)

9. The Drive dropdown menu will list external drives (like USBs) plugged into your computer. If it's empty, that's okay. Plug in your USB, and a name should pop up. It won't be named what your USB is named, but what your laptop calls the USB. 
Note: If you're concerned you don't have the right drive selected, unplug and plug back in your USB. The drive should disappear and reappear.
Note: If you're USB doesn't show up, it's probably just not formatted correctly. Go to the USB formatting instructions!
10. Hit Okay, and wait for the program to finish running. Once it's done, you have a bootable USB! 

### MacOS: Disable Secure Boot to allow dual-booting off of a USB
1. For these next steps, you'll have to reboot your computer, enter recovery mode, and disable secure boot, so you can't have these instructions pulled up at the same time. Probably best to take a photo or write down these instructions.

### Windows: Create Bootable USB

### Windows: Format USB

### Windows: How to Dual-Boot
