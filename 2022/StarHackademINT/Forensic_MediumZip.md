# Forensic : MediumZip

## What is asked

> Crack the password of the zip archive.

## Resolution

To do so I used **zip2john** to get the hash of the password.\
&emsp;`zip2john cracking.zip > zip.hashes`\
After what I used [John](https://www.openwall.com/john/) and the rockyou wordlist to crack the password.\
&emsp;`john --wordlist=/usr/share/wordlists/rockyou.txt zip.hashes`
