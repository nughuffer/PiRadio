# PiRadio

A mashup of programs/scripts that allows random music to be played from a folder and output to an FM channel. 
I had a lot of issues finding a definitive (working) program to do this so this is the result of hours of googling/testing lol.

Connect antenna to pin 7 (gpio 4)

Change frequency in the StartRadio script. The default is 87.9. 

Copy the piradio.service to /etc/systemd/system/ then enable it with:

$sudo systemctl enable piradio 

to have it start after boot up. 

Needs sox, libsox-fmt-mp3, and this program installed to work: 

https://github.com/ChristopheJacquet/PiFmRds

