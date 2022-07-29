# File encryption 

Filesystem level encryption, often called file/folder encryption or stacked level encryption, is a form of disk 
encryption where individual files or directories are encrypted by the file system itself. This is in contrast to full 
disk or block level device encryption where an entire partition or disk, in which the file system resides, is encrypted.

## EFS

Windows built-in Encrypting File System (EFS) is a tool that can encrypt all Windows files and folders on NTFS drives.
It allows you to encrypt a specific folder rather than the [whole hard drive partition](disk-encryption.md). And if you 
move a file to an EFS-encrypted folder, the file will automatically be encrypted.

To enable the EFS tool:

* Open an elevated Command Prompt.
* Type (and enter):

```text
fsutil behavior set disableencryption 0
```

To disable this tool, type (and enter):

```text
fsutil behavior set disableencryption 1
```

To encrypt files and folders:

* Right-click on a file or folder and click Properties.
* Click the Advanced button in the next window.
* Check the Encrypt contents to secure data box and click OK.

## VeraCrypt

[VeraCrypt](https://www.veracrypt.fr/en/Home.html) is a fork of the discontinued TrueCrypt project. It is a free and 
open-source utility for on-the-fly encryption (OTFE). The software can create a virtual encrypted disk that works just 
like a regular disk but within a file. It can also encrypt a partition or (in Windows) the entire storage device with 
pre-boot authentication.



