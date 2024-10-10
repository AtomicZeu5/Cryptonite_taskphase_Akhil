# OASIS CTF
During this cpature-the-flag event, I completed 8 challenges. Those are:

## READY PLAYER ONE
In this, an audio file was given which had beeps in different time gaps. I figured it was morse code and ran it through a morse code translator online and found the flag: `OASISM0R5EM4N1PU7470R` The key was: OASIS{M0R5E_M4N1PU7470R}

## Arte-miss
As the darkness recedes, Halliday's voice echoes with the chilling news that Innovative Online Industries (IOI) has seized control of the OASIS. A virus has infected the main server, sparking widespread panic as players lose their progress. Amidst the chaos, Artemis materializes before you, her avatar flickering erratically. With a sense of urgency, she thrusts a file into your hand and whispers something unintelligible before dissolving into a cascade of pixels. Stunned and disoriented, you scrutinize the mysterious file, desperate to understand its significance. Just then, a calming voice cuts through the turmoilâ€”it's Artemis, speaking from the real world. She reveals that the file holds the key to liberating the OASIS from IOI's grip. Though she was captured and her character deleted, she managed to pass this vital piece of information to you in a final act of defiance. Find the flag hidden in the file.

https://drive.proton.me/urls/VDMJTAVBH4#nCpqsQV4fGjN

This link contains a file. In the hint, it stated that the flag was hidden within the image, so I tried to obtain its metadata and found out that the author of the image was named `OASIS{m4ta_af_04515}` hence, the flag

## String me to sleep
The flag is hidden inside the book, we have to find it. I used `ctrl+f` to search for `OASIS{` to find and found out the key was `OASIS{y0u_fou7d_m3} `

## Jekylle and Hide!

In this challenge, we are given a link https://jekylle-and-hide.oasis.cryptonite.live/. Opening this takes us into a virtual library of sorts. In the hint, they menton the work `inspect` so my first thought was to Inspect element every part of the page as it said the key was split into 2 parts. Inspecting revealed the first half of the key, then I input this as the username which it accepted and asked for a password. Then, when browsing through more data in the inspect element window revealed a set of numbers which looked like a password. I entered this and got the second half of the key. The key was `OASIS{th15_15_part1_!nd_h3r3_go35_1h3_n3xt!!}`

## Keynough is enough

In this challenge, we are given a cipher-looking text. They oddly mention vinegar in the description and this sounded like a hint towards using the Vigenère Cipher. Hence, the key word turned out to be ARTEMIS as it was in caps. I ran it through a  Vigenère cipher decoder with ARTEMIS as the key and found the flag `OASIS{S1L3N7_V1G3N3R3}` 

Couldn't attempt more as I was sick since the weekend and I stopped here
