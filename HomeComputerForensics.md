# Home Computer Forensics

* **Category:** easier
* **Points:** 2

## Challenge

Blunderbussing your way through the decision making process, you figure that one is as good as the other and that further research into the importance of Work Life balance is of little interest to you. You're the decider after all. You confidently use the credentials to access the "Home Computer."

Something called "desktop" presents itself, displaying a fascinating round and bumpy creature (much like yourself) labeled  "cauliflower 4 work - GAN post."  Your 40 hearts skip a beat.  It looks somewhat like your neighbors on XiXaX3.   ..Ah XiXaX3... You'd spend summers there at the beach, an awkward kid from ObarPool on a family vacation, yearning, but without nerve, to talk to those cool sophisticated locals.

So are these "Cauliflowers" earthlings? Not at all the unrelatable bipeds you imagined them to be.  Will they be at the party?  Hopefully SarahH has left some other work data on her home computer for you to learn more.

## Solution

Used powershell commands ```Get-Item credentials.txt -Stream * ``` to find the alternate data stream of ```FILE0```
Then, it required some scripting to extract the alternate data stream file into an image (.png) file. 
```
$file = Get-Content credentials.txt -Stream 'FILE0' -Encoding Byte -ReadCount 0
Set-Content 'file0.png' -Encoding Byte -Value $file
```
Go back to the folder in your file system to find the image file extracted with the flag!
```
CTF{congratsyoufoundmycreds}
```
