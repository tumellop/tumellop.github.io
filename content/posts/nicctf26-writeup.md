+++
date = '2026-01-28T19:47:57+02:00'
draft = false
title = 'NIC CTF26 Writeup'
author = 'prxncessZA'
tags = ["CTF", "Cybersecurity", "NICCTF"]
summary = "At the end of January 2026, **Namibiam International Cybersecurity Conference (NICC)** released a Jeopardy-style ctf **(NIC CTF26)**.However I ended up coming 30th..."
+++

At the end of January 2026, **Namibiam International Cybersecurity Conference (NICC)** released a Jeopardy-style ctf **(NIC CTF26)**.However I ended up coming 30th, missing out on a Top 10 spot. Here are some of my writeups

## 📂 MISCELLANEOUS

## 1. Welcome (10 Points)
**Author:** John_x9  
**Flag Format:** `NICCTF26{...}`

### Description
> my bot:  
> Discord server [https://discord.gg/NNcdgJx5C]

### Solution
In this challenge, I had to join the Discord server. I found the `#Welcome` channel, which gave me the first clue.

![Welcome Clue](/images/welcomeClue.jpeg)

After analyzing the history of the channel, I ended up investigating the bot's profile. The flag was hidden in the bot's roles.

![Discord Bot Profile](/images/discordBot.jpeg)

**Flag:** `NICCTF26{heh_zzzrt}`

---

## 🕵️ OSINT

## 1. Long Distance Friend (100 Points)
**Author:** Sen0i  

### Description
> I want to meet my friend. The only thing I remember is the old photo he once gave me the entrance of his house. Find the location where he is residing.  
> **Format:** `NICCTF26{Casagrand_Asta}`

![Entrance Photo](/images/image.png)

### Solution
We were given an old photo of the entrance to a friend’s house. I used **Google Lens** on the image, which quickly identified the building as **Rustomjee Seasons** in Bandra East, Mumbai.

**Flag:** `NICCTF26{Bandra_East}`

---

## 2. Bruhh!! It's CHISHIYA🗿 (100 Points)
**Author:** Sen0i

### Description
> A player named `shuntaro_.chishiya_` holds the flag in the Borderland. He doesn’t run. He doesn’t bluff. He waits silent, calculating, always ahead. Can you get the flag from him?

### Solution
I searched the name on Google and found an Instagram account with that username.

![Instagram Profile](/images/shinsta.png)

Scrolling through the first post, I noticed a faint, faded text in the top-left corner. That was the flag.

![Hidden Text](/images/hidden.jpeg)

**Flag:** `NICCTF26{but_1m_cl3v3r}`

---

## 3. Cockpit Climb (200 Points)
**Author:** John_x9

### Description
> The Palm Springs Air Museum offers rare up-close access to some of aviation’s most iconic aircraft. This image comes from that collection. Your task is simple: identify the aircraft shown.
>
> **Flag format:** `NICCTF26{Aircraft_Name}`

![Aircraft Image](/images/c.jpeg)

### Solution
For this challenge, I ran the image through **Google Lens**, and it recognized the aircraft as a **Lockheed F-104 Starfighter**.

**Flag:** `NICCTF26{F-104 Starfighter}`

---

## 4. Finding Beagle (200 Points)
**Author:** Sen0i

### Description
> I walked into a pet shop one day and saw the cutest beagle ever… but didn’t buy it. Now I regret it — and I want to call them back. The problem? I forgot the shop’s name and didn’t save their number. All I know is, the place in the picture was near the shop. Help me find it—and get their number.
>
> **Flag format:** `NICCTF26{xxxxxxxxxx}`

![Location Tower](/images/location.jpg)

### Solution
For this challenge, I placed the image of the tower into Google Lens and it identified it as the **Dehradun Clock Tower** (also locally known as "Ghanta Ghar").

I then went to the Dehradun Clock Tower on Google Maps and simply searched for "pet shop". I found **Dehradunpetdogs**.

![Pet Shop Result](/images/petshop.jpeg)

Their phone number was listed in the business info: `+917668669112`.

**Flag:** `NICCTF26{7668669112}`

