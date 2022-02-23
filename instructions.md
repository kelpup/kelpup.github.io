# Windows Instructions for Burning Our ISO

### Introduction - What is an ISO?
We say that you can "burn our ISO" onto a flashdrive, and use that to run our disro on your computer. But what does that really mean? 

> "The idea behind an ISO imge is that you can archive an exact digital copy of a disc, and then later use that image to burn a new disc that's in turn an exact copy of the original (...) most operating systems allow you to mount an ISO image as a virtual disc, in which case all your apps treat it as if a real optical disc were inserted." - ([source](https://www.howtogeek.com/356714/what-is-an-iso-file-and-how-do-i-open-one/))

So when you download our ISO file, it is really just a copy of the linux distrubtion we have created. By "burning" it onto a flashdrive, you are just making your own portable copy that you can then insert and boot on your own machine.

### What You'll Need
```markdown
- A 4GB or larger flashdrive
- Microsoft Windows
- [Rufus](https://rufus.ie/en/), a third party ISO burning application
- [Kelpup](), our personalized Linux distro's ISO image
```

### Step 1 - Download Rufus

Following the link above to Rufus' website, navigate to the large "download" button near the top of the home page. 

<img src="Windows Instructions/DownloadRufus.PNG" alt="Rufus Download Button" class="inline"/>

Click the button and boot up the software. 

### Step 2 - Choosing USB Device

Upon booting up the software, the following option menu will greet you:

<img src="Windows Instructions/SelectUSB.png" alt="Selecting a USB within Rufus" class="inline" height="350"/>

The first step is to let Rufus know what device you'll be burning to. To do this, plug in your external USB, and navigate to the "Device" field of the menu. From there, select your personal USB. 

### Step 3 - Download and Select the Kelpup Linux Distro as Your ISO File

Use this [Link](https://github.com/orgs/kelpup/repositories) to download our ISO. Make sure to download the file to somewhere you will remember. Then, click on the "Select" drop down to the right of the Boot Selection menu. 

<img src="Windows Instructions/SelectISO.png" alt="Selecting an ISO within Rufus" class="inline" height="350"/>

Navigate to your Kelpup download, and select "open". 

### Step 4 - Burn the ISO

Click on the "Start" button, leaving all other settings at default. 

<img src="Windows Instructions/Start.PNG" alt="Start the ISO burning Process" class="inline" height="350"/>

#### You may encounter additional warnings or pop ups after pressing start:
```markdown
# "Download Required":
  - Rufus requires supplemental files to burn your ISO. 
  - Simply press "Ok" to resolve the issue.
  - More files will be installed. 
# "ISOHybrid Image Detected":
  - Rufus recognizes your ISO as being compatable with aditional discs. 
  - Simply select the "Write in ISO Image Mode" bubble to continue. 
  - It will be the recommended / default option. 
# "Data Destruction Warning":
  - All previous contents on the USB will be overwritten. 
  - If this is not acceptable, select a new device. 
  - Otherwise, simply press "Ok" 
```

While the ISO burns, you will see a status bar that shows progress. Most ISO burnings will take ~10 minutes. 

<img src="Windows Instructions/Status.png" alt="Rufus Status Bar" class="inline" height="350"/>

### Step 4 - Using the ISO

When the progress bar fills, you can select "Close" and quit Rufus. To use the ISO, simply insert it into an external port on your Windows computer, reset your computer, and pull up the BIOS menu. Typcially you can do this using one of the following hotkeys, depending on your version of BIOS:
- ESC
- F1
- F2
- F8
- F10

Choose to enter BIOS Setup, and the following utility page will appear:

<img src="Windows Instructions/BIOS.PNG" alt="BIOS Menu" class="inline"/>

Navigate to the "Boot" tab. All of your avalible system devices will be displayed here in the order of their priority. To run Kelpup Linux, you will have to move it such that it is number one in the list. When you have done this, your computer will automatically reboot an run Kelpie Puppy Linux!
