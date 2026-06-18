
# PsyduckGotchi (Tamagotchi Project)

Psyduck-gotchi (gotchu!) is a my very first project I ever made for fallout. I made this using the tamagotchi tutorial on the fallout site!
A tamagotchi is basically a virtual pet you can take care of with stats indicating it's happiness, energy and hunger. It's a silly little thing that you can bring around and make you feel like you're taking care of something, Psyduck runs off an ESP32 with LIPO battery compatibility

# How this works!
My tamagotchi project has 3 buttons, an LCD screen, a buzzer, and has neopixels for the LED backlighting. 
When you first boot up the OLED display, it should contain the Energy, Happiness and Hunger stats on the screen. 

<img width="829" height="789" alt="image" src="https://github.com/user-attachments/assets/8570eb29-d427-4466-b80f-a2b9655185b5" />

3 different screens will be played on the OLED. If psyduck looks happy, it means that one of your stats (happiness, energy, hunger) is above 60. If psyduck is neutral than your stats are between 60 and 30 (should be fine, leave him alone for a bit!). If psyduck is sad then all of your stats are below 30%.
Careful! Psyduck can die ... :(. If all of your stats are under 5% then psyduck will die!! Don't worry though, he's not dead forever, just for a minute, after that his stats return to normal again!

the 3 buttons on the tamagotchi do as follows:
Left button: Feed the duck
              - When you press the button, the virtual pet will be fed! Used when hunger bar is low 
Middle button: Play with the duck
              - When you press the middle button, the you can play with the virtual pet! This is used when the happiness bar is low
Right button: Put the duck to sleep
              - When you press the middle button, you will put the duck to sleep, a sleeping image is played! This is used when the energy is low

Everytime a button is clicked, the buzzer will play a sound.

# why I made this

I made this project since I thought it would be a super good first hardware project instead of making hackpads like everyone else. I also made this since I thought 
it would be a challenge for me to CAD since I had previous CAD experience. This is also a birthday present for a friend who looooves psyduck ( a very very cute and stupid pokemon). It's stereotypical that
I try to buy something psyduck themed but I thought since I had the 3D printer filament, why not go for a psyduck printed item (oops I hope I have enough filament).

Here's the ONshape model of my project assembled, casing and all! (Psyduck doesn't really look like psyduck BUT I TRIED)

<img width="796" height="688" alt="image" src="https://github.com/user-attachments/assets/94a34cbd-ea2a-4e88-98b3-6e21f1710bc2" />


# PCB
Here's the wiring schematic and traces of my PCB as well as a kicad's 3D render

<img width="918" height="637" alt="image" src="https://github.com/user-attachments/assets/b0712de8-4f3a-40f0-9cba-d861c2f9dcb8" />

Schematic ^^

<img width="665" height="571" alt="image" src="https://github.com/user-attachments/assets/8d5bd0e8-c1b9-4163-b08d-260aacc32216" />

Traces^^

<img width="704" height="535" alt="image" src="https://github.com/user-attachments/assets/bfa05090-e594-4de2-ab6b-fa82fc7c4964" />

3D render^^

# BOM (bill of materials)
[Tamagotchi BOM - Sheet1.csv](https://github.com/user-attachments/files/29111727/Tamagotchi.BOM.-.Sheet1.csv)

Item| Description| Quantity (#)| Unit price ($)| Shipping($)| Total Price ($)

PCB|PCB quote from JLCPCB|1|$2.00|$2.50|$4.50
ESP32,Seed Studio XIAO ESP32,,1,$4.94,$18.31,#VALUE!
OLED,128 x 64 OLED LCD,,1,$4.00,,$4.00
Buzzer,Passive Buzzer,,5,$0.06,,$0.50
Buttons,Hropart round buttons,,5,$0.11,,$0.50
LED,Yongyutai LED's,,50,$0.01,,$0.50
LCSC shipping,,,,,$14.51,
Total,,,,,35.32,$45.32




