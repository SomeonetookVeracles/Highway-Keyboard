---
title: "HC Standard Keyboard"
author: "Owen Borgos, or Veracles"
description: "This will be a standard 100% keyboard design, with a screen and rotary encoder, as well as an SD card reader.
created_at: "2025-06-5"
---

# June 8th, began designing PCB

(Quick note, I lost all my progress about halfway through, and rebuilt it, so all of these first entries are sparser, pls read to the end for the real journal!)
Created chip, clock, and wiring, will do sd card reader and USB-c tomorrow.
![image](https://github.com/user-attachments/assets/d8759672-2006-4f70-8dd5-96b3a1e44f10)

**Total time spent: 2.5 Hours**

# June 9th, WHY WONT SWITCHES APPEAR
Added USB-C, But for some reason the SWITCHES WONT APPEAR. (I found out after this that the switches that show up in the kicad plugin manager are PCB only, your just supposed to use a generic switch symbol...)
![image](https://github.com/user-attachments/assets/329a5ef9-bbfa-4b90-961a-25bde960e894)

**Total time spent: 3.5 Hours**

# June 22nd, Finally fixed the great switch dilemma
I got switches working finally, and got them mapped to the blueprint:
![image](https://github.com/user-attachments/assets/fdd17c3e-02b0-4999-93bd-8fcc88a5c510)

**Total time spent: 5 Hours**

# June 23rd, Added some cool stuff
Playing around with using through holes and hand soldering to give me more flexibility with an OLED Screen and Rotary encoder, will update if there's progress.
I also added a MCP 23017 to give me additional GPIO for fun stuff like the screen and encoder.
![image](https://github.com/user-attachments/assets/0416864c-c5ca-47bf-8bf3-cff038e2f550)

**Total time spent: 7 Hours**

# July 21st, Redid a ton of stuff
I reinstalled windows on my computer and lost literally all of my data, including my backups, and the github version was corrupted for some reason, so I decided to rebuild the board from scratch, using a few new tricks I learned from my business card PCB I did as a distraction.
<img width="1419" height="726" alt="image" src="https://github.com/user-attachments/assets/945f4ad2-e5fc-4622-b86c-56436edeff51" />
It's a bit (super duper) cursed, but I got most of the wiring done:
<img width="1048" height="558" alt="image" src="https://github.com/user-attachments/assets/8c9b42ce-01c1-40a4-81f9-9509f0d764de" />
FINALLY GOT IT TOGETHER, I'M GONNA LOSE MY MIND
<img width="1111" height="505" alt="image" src="https://github.com/user-attachments/assets/6e2e1a11-8586-473d-a292-b07d6ca49faf" />
I also added a few more holes for screws, for added stability, these'll be added using heat threaded inserts, as I have a few spare I accidentally stole from my school.
<img width="661" height="318" alt="image" src="https://github.com/user-attachments/assets/abd2baff-e6b4-470e-a9a1-47a1c9c9b67b" />

I then did the case, this took a while (3 hours) because I had to manually cut out the holes for each switch, and fiddle with the tolerances on it so it would fit better later on.
<img width="1437" height="790" alt="image" src="https://github.com/user-attachments/assets/0bc5855b-08bf-46c7-9e4e-affcbe1e0b0a" />

I FINISHED THE CASE! (The holes for the switches are there I had to suppress them because of lag :sob:)
<img width="1324" height="766" alt="image" src="https://github.com/user-attachments/assets/4541fe62-a9df-4143-8fb2-0978045e1f81" />

**Total time spent: 19 hours**

