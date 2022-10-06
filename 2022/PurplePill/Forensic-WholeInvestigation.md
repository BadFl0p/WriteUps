# Forensic : Whole Investigation

## What is asked :

> Find the IP and port inside the disk image.

## Resolution :

First I extracted the content with `binwalk`. I had a look at every thing inside the extracted folder and looking at the *ab2b61150214b18be42294c2b9da3aeafc2b4d7c041ed7b4277e9f65b4123b65* folder there was a tar archive.
In which there was some directory related to a Linux machine (etc, root). Inside the **etc** directory we find the configuration for `cron` indicating a cronjob with the following string */dev/tcp/1.3.3.7/1337*.\
Therefore the flag is *PPCTF{1.3.3.7:1337}*.
