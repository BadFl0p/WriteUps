# Forensic : Data Exfiltration

## What is asked

> Find the data which was exfiltrated.

## Resolution

I never worked with data exfiltration so the first thing to do was to learn about it with [this](https://www.youtube.com/watch?v=0Fn3VD3_ZPA) video.
But looking at the pcap the TCP traffic didn't seems to store any data, but on the other hand there was a bunch of DNS traffic.
So I had a quick look at [this](https://www.youtube.com/watch?v=ftCy-seCNjc) which guided me to decode the string of the subnet domain of each DNS query.\
The result looked like some base64 string, decoding it gave me the flag.
