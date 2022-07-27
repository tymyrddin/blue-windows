# Enable full disk encryption using BitLocker

Enabling full disk encryption minimizes the chance that data on your computer will ever be misused. 

## Requirements

* Windows 10 Pro and Windows 10 Enterprise include BitLocker, Windows 10 Home does not. 
* A TPM chip. To check if your machine has a TPM chip:
  * Type tpm.msc in the search box, and press enter. 
  * In the following window, check the TPM status.

On some systems, TPM chips are disabled by default, and you will need to enable the chip in the BIOS menu: Under 
Security settings, look for a TPM subsection. Most likely it will allow Activation/Enabling by ticking some box
or a toggle of sorts. If there is no TPM chip on your motherboard, you can still enable Bitlocker by editing the 
"Require additional authentication at startup" group policy.

## Enable via Control Panel

* Either Control Panel -> Bitlocker Drive Encryption OR System and Security -> Bitlocker Drive Encryption
* Expand the drive you want to enable Bitlocker on, and click on the Turn on Bitlocker hyperlink
* If your TPM is already enabled, you will directly be brought to the BitLocker Startup Preferences selection window. If not:
  * Go through the Bitlocker Drive Encryption startup by clicking on Next. Eject any connected USB drives and remove any CDS/DVDs sitting idle in the optical disc drive. Click on Shutdown.
  * Follow the instructions that appear on the screen to activate the TPM. Activating the module is as simple as pressing a key (varies depending on manufacturer). 
  * The computer will most likely shut down again once you activate the TPM; turn on your computer back on.
* Choose to enter a password at every startup or connect a USB/Flash drive (Smart Card) containing the startup key. The latter is somewhat of a dangerous option. If the USB drive holding the key is damaged or lost you may lose access to the drive.
* Set a [strong password](../authentication/passwords.md) and re-enter it to confirm. Next.
* Keep the recovery key securely locked away on both (dedicated) USB storage and paper.
* Choose to either encrypt the entire hard drive or only the part used. 
  * On old buckets where most of the storage space is already being used, do the whole hard drive.
  * On new machines, or machines with little data, choose to encrypt only the space that is currently filled with data. Bitlocker will automatically encrypt any new data you add to the disk.
* Choose encryption modes. 
  * Select the New encryption mode if the disk is a fixed one.
  * Select compatible mode if you are encrypting a removable hard drive or USB flash drive.
* Depending on your system 
  * Run BitLocker system check (OR)
  * Start encrypting
* Restart the computer to initiate the encryption process (can take from 20 minutes to hours)

Now every time you boot on your computer, you will be prompted to enter the passkey in order to access the encrypted 
files.

