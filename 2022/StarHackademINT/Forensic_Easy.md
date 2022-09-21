# Forensic : Easy

## What is asked

> Read the disk image to find the file which contains the flag.

## Resolution

I decompressed the archive I downloaded and got a *.raw* file.\
In the terminal I used `binwalk -e file.raw`, giving me a directory of the files that binwalk extracted from the raw file. Inside this directory there is a txt file which contains the flag.
