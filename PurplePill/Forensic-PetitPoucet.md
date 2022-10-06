# Forensic : Petit Poucet

## What is asked

> Find the flag inside the pcap file.

## Resolution

I started looking at the object we could export from the capture but there was nothing interesting.\
Then looking at the protocol hierarchy I saw that it was mainly HTTP so I guessed I should just have a look at all the packets.
After some time, I saw the string *PPCTF{F0ll0W_TCP}* hidden in the last HTTP packet at the end of some js code.
