# How to make a bootable macOS installer

 - Plug in an external drive with at least 8GB space (preferably 12GB) as that’s how much the installer will require.
 - Launch Disk Utility (press Cmd + spacebar and start to type Disk Utility).
   - Before this next step - if you are running High Sierra you will need to click on the View drop down below the close minimise buttons.    - Choose Show All Devices from the options. Now you will see the external root drive in addition to the volume below it.
 - Select the root drive in the sidebar (the next step won't with if you only select the volume).
 - Click on Erase.
   - Choose Mac OS Extended (Journaled) as the Format.
   - Choose GUID Partition Map as the Scheme.
     - Your drive will be called `Untitled` by default.
   - Click on Erase.
 - Wait while Disk Uitlity creates the partition and sets up the drive (this can take a few minutes).
 - Then click Done.
 
 ## Terminal command
 `sudo /Applications/Install\ macOS\ High\ Sierra.app/Contents/Resources/createinstallmedia --volume /Volumes/Untitled --applicationpath /Applications/Install\ macOS\ High\ Sierra.app`
 - It takes time to run, wait a few minutes for the "done" messages to appear.
