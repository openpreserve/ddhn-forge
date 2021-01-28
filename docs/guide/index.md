# User's Guide
Here we provide help for users who are new to VirtualBox and using virtual machines. The guide isn't

## Starting VRE
Following [installation](/setup) the normal start up procedure is to open the Virtualbox Manager window, the left side of which will contain the DDHN VRE virtual machine icon which will be in the powered off state.
To start, select the VRE icon and then the green start arrow on the top menu selecting ‘Normal Start’ - this will open the virtual machine and the VRE display window.
Note the Virtualbox Manager is also used for managing / configuring Virtualbox settings  - further details can be found on the Oracle Virtualbox user guide

**Resources**

- [Starting Virtualbox](https://www.virtualbox.org/manual/ch01.html#intro-starting)

## Using VRE
The VRE default desktop environment is GNOME 3 based. For users unfamiliar with GNOME the simple user guide can be found via the following link [GNOME 3 User guide]( https://help.gnome.org/users/gnome-help/stable/shell-introduction.html.en). The visual guide provides an overview of the Activities menu that is accessed via the top left of the VRE display, this manages access to your windows and applications. When enabled the vertical panel provides access to the DP tools, files as well access to:
* Firefox
* Gnome help
* Gnome terminal - this  terminal emulator and has been set up to provide access to the command line environment
To access and manage the system settings on your desktop use the menu on the top right of the VRE screen. To access general settings select the top right down arrow, there are 3 selection symbols:
* The right side power off symbol this should be used for a graceful VRE shut down
* The padlock symbol locks the application, a vagrant password is needed to reactivate
* The left side symbol provides general settings access
Further details can be found in the GNOME 3 guide.

**Resources**

- [GNOME 3 User guide]( https://help.gnome.org/users/gnome-help/stable/shell-introduction.html.en).

### File Sharing
To make best use of the DP tools you will need access to the files located on your normal operational computer (the host). These files will need to be accessed or shared with the  virtual machine (often referred to as the guest). This is a straightforward, Virtualbox control function. The detail covering set up can be found [online here](https://www.virtualbox.org/manual/ch04.html#sharedfolders).

From the Virtualbox Manager:

1. Ensure that the relevant virtual machine is selected - DDHN VRE. The machine should be powered off
2. Select Settings - This is selected via the Settings icon that is by the Start icon or via the pull down selection menu entitled Machine on the left side of the Virtualbox window immediately above the DDHN VRE virtual machine icon
3. Select the Shared Folders menu. A window will appear. The top right will display the Settings icon with the label DDHN VRE Settings. Above the main body of the window the heading ‘Shared Folders’. To the right side of the main window note a + symbol; select the + symbol this will open a further window
4. This new smaller window is entitled ‘Select Share’ - this will be displayed alongside the Settings icon at the top of the window. The window contains 3 main boxes entitled ‘Folder path’, ‘Folder name’ and ‘Mount point’. Two smaller tick boxes entitled ‘Read only’ and ‘Auto mount’ will also be visible
5. Select Folder path that will allow you to select one of two options. Select ‘Other’
6. A further window will now open that should contain a list of folders located on your host machine. Select the folders that you wish to have access to from your host machine and press ‘Select Folder’. The folders window will close and bring you back to the preceding Select Share window
7. The Select Share window will automatically define the path of the host folder selected. It is recommended that you tick the ‘Read only’ box, this will ensure that you do not inadvertently overwrite a file or folder on the host machine whilst using it on the guest machine.
8. Enable Auto Mount’ - now select ‘OK’
9. Start the DDHN VRE virtual machine - note the new shared folders icon in the virtual machine window

**Resources**

- [Virtualbox shared folders](https://www.virtualbox.org/manual/ch04.html#sharedfolders)
