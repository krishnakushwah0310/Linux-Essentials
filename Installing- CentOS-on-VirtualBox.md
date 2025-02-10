# CentOS Installation on VirtualBox Video

To watch the video for installing CentOS on VirtualBox, click on the link below:

[CentOS Installation on VirtualBox Video](https://www.youtube.com/watch?v=ZqyVrfW2c6g)



# Installing CentOS on VirtualBox

## 1. Download CentOS ISO

   - First, you need to download the CentOS ISO file.
   - Go to the [CentOS Download page](https://www.centos.org/download/), and choose the version (CentOS Stream or CentOS Linux) you want to install.
   - Download the appropriate ISO (usually `x86_64` for most systems).

## 2. Install VirtualBox

   - Download and install VirtualBox from [VirtualBox's official website](https://www.virtualbox.org/).
   - Follow the installation steps according to your OS (Windows, macOS, or Linux).

## 3. Create a New Virtual Machine in VirtualBox

   - Open VirtualBox and click on the **New** button.
   - Choose a name for your virtual machine (e.g., "CentOS").
   - Select the type as **Linux** and the version as **Red Hat (64-bit)** or **CentOS (64-bit)**, depending on the VirtualBox options.
   - Click **Next**.

## 4. Allocate RAM

   - Choose the amount of RAM for your virtual machine. A good starting point is 2GB or more, depending on your system's available RAM.
   - Click **Next**.

## 5. Create a Virtual Hard Disk

   - Choose **Create a virtual hard disk now** and click **Create**.
   - Select the **VDI (VirtualBox Disk Image)** option and click **Next**.
   - Choose **Dynamically allocated** so that the disk size grows as needed.
   - Set the size for the virtual hard disk (e.g., 20GB or more) and click **Create**.

## 6. Attach the CentOS ISO to the Virtual Machine

   - Select your new VM and click on **Settings**.
   - Go to the **Storage** tab.
   - Under **Controller: IDE**, click the empty disk icon, and then on the disk icon on the right side, click **Choose a disk file**.
   - Select the CentOS ISO file you downloaded earlier.
   - Click **OK** to save the settings.

## 7. Start the Virtual Machine

   - With your virtual machine selected, click on the **Start** button.
   - The virtual machine will boot from the CentOS ISO, and you will see the CentOS installation screen.

## 8. Install CentOS

   - Once the system boots from the ISO, select **Install CentOS**.
   - Follow the same installation steps as on a physical machine:
     - Select your **language** and **keyboard layout**.
     - Set the **time zone** and **root password**.
     - Select the hard drive and set up partitions (either automatic or manual).
     - Start the installation process by clicking **Begin Installation**.

## 9. Finish Installation

   - Once the installation is complete, the system will prompt you to reboot. Before rebooting, make sure to remove the CentOS ISO from the **Virtual CD/DVD** disk in the VM settings, or it will boot from the ISO again.
   - Click **Reboot**.

## 10. Post-Installation

   - After the first reboot, CentOS will finalize its setup.
   - Log in with your root password or the user account you created.
   - It’s always a good idea to update the system after installation. Open the terminal and run:
     ```bash
     sudo dnf update
     ```

## 11. Install VirtualBox Guest Additions (Optional)

   - After the installation, you can install **VirtualBox Guest Additions** for better integration, such as clipboard sharing, improved graphics, and seamless window resizing.
   - With the VM running, click on **Devices** in the VirtualBox menu, then click on **Insert Guest Additions CD image**.
   - Follow the instructions to install the Guest Additions inside the CentOS VM.
