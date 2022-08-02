# Check integrity of downloads

When downloading an ISO image of, for example, the latest Linux distro, installing or upgrading packages, or 
downloading software, you can verify the files have downloaded correctly and securely by using checksums. 
Checksums ensure the integrity of data portions for data transmission or storage. Checksums is a simple error-detection 
scheme in which each transmitted message is accompanied by a numerical value based on the number of set bits in the 
message. The receiving station then applies the same formula to the message and checks to make sure the accompanying 
numerical value is the same. If not, the receiver can assume that the message has been garbled (or was altered).

## Verifying downloaded software

When downloading software, `.iso`s and `.deb`s and the like, download the `xxxsum` (choose from what is available) as well as the software and check. 

Open Command Prompt or PowerShell and type:

    > certutil -hashfile [file_name] [hash-algorithm]

For example:

    > certutil -hashfile .\some-file.iso sha256sum

and compare the output from the command with the key listed in the associated `sha256` file.
