# The Console Liberation Guide: The Definitive Walkthrough for Modding a PlayStation 2

## Part 1: The Philosophy - What Are We Doing and Why?

Welcome to one of the most rewarding projects in classic console modification. We are about to unlock the true potential of the legendary PlayStation 2. But before we touch any hardware, it's crucial to understand *what* we're doing and *why* it works.

**What is Free McBoot (FMCB)?**

Free McBoot is not a "hack" in the traditional sense. It is a brilliant piece of software that takes advantage of a feature Sony itself designed: the ability for the PS2 to launch applications directly from the memory card upon startup. The PS2's BIOS contains a list of files to look for. FMCB is simply a custom-built, independent operating system that we install onto a memory card. When the PS2 boots, it sees this special file on the card and launches our custom OS instead of the standard Sony browser.

**Why does this give us so much power?**

The standard Sony OS only allows you to play official game discs and manage saves. Our new FMCB operating system is designed for freedom. It allows us to launch other, more powerful homebrew applications—programs created by the community. The most important of these is **Open PS2 Loader (OPL)**, an application that can load and play game backups directly from a USB drive or an internal hard drive.

**Our Goal:** Install FMCB onto a memory card. Then, use FMCB to launch OPL. Then, use OPL to play games from a USB drive.

This guide will be meticulous because messing with console hardware and software requires precision. Let's begin.

---

### **Part 2: The Arsenal - What You Will Need**

This process has very specific requirements. Gather everything before you start.

1.  **A PlayStation 2 Console:** This guide is primarily for the original "Phat" models and most "Slim" models (pre-SCPH-90000 series). The very last Slim models removed the key vulnerability.
2.  **An Official Sony 8MB Memory Card:** While some third-party cards work, many fail during the installation. For the highest chance of success, use an original Sony 8MB card for the FMCB installation. You can use any card for game saves.
3.  **A Method to Run the Installer:** This is the trickiest part. To install FMCB onto a memory card, you first need a way to run the installer program on your PS2. There are a few ways to do this:
    *   **The Swap Magic Method:** Requires owning Swap Magic discs.
    *   **The Modchip Method:** Requires having a modded PS2 already.
    *   **The "Friend" Method:** If you have a friend with an already modded PS2, you can install FMCB on your card using their console.
    *   **The "007 Agent Under Fire" Method (Our Focus):** This is a clever software exploit using a specific version of a specific game. We will focus on this as it only requires a specific game disc.

4.  **A USB Flash Drive:** Formatted to FAT32. This will hold our installer files.
5.  **A Specific Game Disc:** For our chosen method, you need a copy of **James Bond 007: Agent Under Fire**. It *must* be the original black-label version, not the "Greatest Hits" red-label version, as the exploit was patched.

[image: A high-quality photo showing all the required components neatly laid out: the PS2 console, the official 8MB memory card, the USB drive, and the specific black-label copy of the game disc.]

---

### **Part 3: The Preparation - Setting Up Your USB Drive**

We will now prepare the files needed for the exploit and installation.

1.  **Format Your USB Drive:** Plug your USB drive into your computer. Right-click on it, select `Format...`, and ensure the file system is set to **`FAT32`**. This is non-negotiable, as the PS2 cannot read other formats.
2.  **Download the "FreeDVDBoot" Exploit:** This is the file that will trick the game's DVD player into launching our installer. Download the correct file for your game from the official FreeDVDBoot GitHub repository.
3.  **Download the FMCB Installer:** Go to the official FMCB release thread on the PSX-Place forums and download the latest version of the installer.
4.  **Organize Your USB Drive:**
    *   Create a folder named `APPS` on your USB drive. Unzip the FMCB installer and place all of its contents inside this `APPS` folder. The key file is `FMCBInstaller.elf`.
    *   Now, handle the FreeDVDBoot exploit. Depending on the version, you might need to burn it to a DVD-R. For the "Agent Under Fire" method, there's often a specific save file exploit. You would place this specially crafted game save file in the correct folder structure that the PS2 can recognize.

[image: A screenshot of a computer's file explorer showing the USB drive's folder structure, with the `APPS` folder containing the FMCB installer files clearly visible.]

---

### **Part 4: The Execution - The "Agent Under Fire" Exploit**

This is the most delicate part of the process. Follow it exactly.

1.  **Insert Peripherals:** Plug your controller and the blank 8MB Memory Card into your PS2. Do **not** insert the USB drive yet.
2.  **Launch the Game:** Insert your "Agent Under Fire" game disc and start the PS2. Let it boot into the game.
3.  **Load the Exploited Level:** Navigate through the game's menus to a specific level as instructed by the exploit's documentation. This usually involves loading a mission or a specific save file that has been crafted to trigger the exploit.
4.  **Trigger the Exploit:** At a specific point in the level, you will perform a specific action (e.g., drive into a certain wall, look at a certain object). If done correctly, the game will "crash," but instead of freezing, the screen will go black and then display a new menu. This is the exploit working.
5.  **Launch the Installer:** This new menu is a temporary launcher. Now, carefully insert your **USB drive**. Navigate the menu to `mass:/` (this is your USB drive) and then into the `APPS` folder. Find and select **`FMCBInstaller.elf`**.

[image: A photo of the TV screen showing the game just before the exploit is triggered, or the special menu that appears after the exploit is successful.]

---

### **Part 5: The Installation - Creating Your Magic Memory Card**

You are now in the FMCB Installer. The hard part is over.

1.  **Select Your Options:** The menu is straightforward. You will have options like "Install," "Multi-Install," and "Format MC."
2.  **Format First:** It is highly recommended to select **`Format MC`** first to ensure your memory card is clean.
3.  **Choose "Install":** Select the standard "Install" option. This will install FMCB onto your card. The process takes a few minutes. You will see a log of all the files being written.
4.  **Success!** Once the installation is complete, you will see a success message. You can now exit the installer and power down your PS2.

[image: A clear photo of the FMCB Installer menu on the TV screen, with the "Install" option highlighted.]

---

### **Part 6: The Liberation - Your First Boot**

This is the moment of truth.

1.  Remove the game disc and the USB drive. The only thing in your PS2 should be your newly created FMCB Memory Card and a controller.
2.  Turn on the PS2.
3.  Instead of the usual "Browser/System Configuration" screen, you will see the beautiful, custom **Free McBoot logo**, followed by a new main menu.

Congratulations. Your console is now liberated. From this menu, you can launch OPL, emulate older consoles, manage files, and so much more. You have taken a closed system and opened it up to a world of new possibilities.

[image: A final, triumphant photo of a TV screen displaying the Free McBoot main menu.]
