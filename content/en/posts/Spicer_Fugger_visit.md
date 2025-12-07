---
title: 'A Visit From Fugger and Spicer'
date: 2025-12-03T12:40:44-08:00
draft: false
tags: [Visit]
author: "Zander Ray"
featured_image: "https://cdn.osuoverclocking.com/spicer_fugger/Group_shot.webp"
description: "Going over collaboration with established members of the XOC Community"
---

# Goals

With this collaboration we aimed for acquiring knowledge and best practices to add to our own. We Sought this by having Charles Wirth (Fugger) and Max Spicer (Spicer) fly up to do benching on some platforms we share.These platforms would be: Arrow Lake (Intel), AM5 (AMD), and Sapphire Rapids (Intel).

---

# Memory Overclocking

![Spicer Teaching](https://cdn.osuoverclocking.com/spicer_fugger/spicer_w_member.webp)

The first of these Arrow Lake we focused on memory frequency validation (mem Valid) this is where we compete to see who can achieve the highest valid frequency for our memory, as of writing the record is 6765.2 mhz. This can lead to some confusion as a lot of kits of ram are sold as "6400 xmp" and that is because that number is the megatransfers per second (mt/s) which is double the number of the actual frequency due to ram modules be DDR or Double Data Rate. So in reality that 6400mt/s kit is 3200 mhz. Working with Spicer we were able to achieve 5512.8 mhz on a ASUS ROG Z890 Apex motherboard and a Intel Core Ultra 7 265k processor using Liquid Nitrogen. The tools and techniques of ths were shared to an audience of members who all took turns pushing the mem kit provided by Patriot to its limit. We used quite a few peripherals supplied by Elmor Labs, like the Hot300 heater and heater plate, Volcano LN2 pot, and the OC Panel, all of which helped to make the process easier and made it a bit more accessible for some of our students to know what is going on, for example those with poor eyesight appreciated the OC panel for the large display out of the post codes in a position that is easier to read.

# AM5 Overclocking

![7950x setup](https://cdn.osuoverclocking.com/spicer_fugger/Am5.webp)

This is fairly new to us, we had interest in learning the AM5 platform due to the global point advantage that ryzen has with some core counts. To quickly summarize, it's an ok OC platform. That is alot of the members found it kind of boring, as Arrow Lake proposes a lot of challenges and thus solutions are needing to be found and executed, however newer members found these chips easier to pick and as they are quite simple. There are some interesting things that we found with AM5 is that there are some voltage rails like Arrow lake's SOC voltage that lower the cold bug temp, in our case our Ryzen 9 7950x's cold bug was removed entirely allowing us to full pot. However this seemed to harm performance by reducing score by ~2%. There is also similar in depth tuning that we have as of writing learning that was brought up by Spicer, that being the dual CCD and optimizing the infinity fabric clocks. The latter is something we have known about but given new information on feed voltages we are now better equipped to tune the infinity fabric clock further.

# Modern HEDT

![Setup of w9](https://cdn.osuoverclocking.com/spicer_fugger/pre_run.webp)

One of my favorite segments of the desktop space is HEDT and the last true HEDT chip we got from intel was the x299 platform and the 10980XE (My favorite chip of them all), however there is a crazy chip they released not too long ago the W9 3495x overclockable 56 core 112 thread Xeon. I have run it only a handful of times and each time the power draw was well into 2kW. This also makes it more challenging as cold bug sits around -50C to -60C meaning you don't get much of a temperature delta between the chip package and the cold bug limit. This means cooling efficiency is key, making this platform more dependant then most on heat transfer and thermodynamics, and as a Mechanical Engineering major that makes me excited for a challenge like this. Due to the massive power dissipation we used a Elmor Labs Volcano X LN2 pot, and made sure to have a dedicated person ready to refill flasks of LN2 to feed it. We had plenty of power on tap with two 2200W PSU's. With that our ASUS Pro WS W790E-SAGE SE helped us set the highest score in Geekbench AI as of writing. This was very muc possible due to learning from Fugger who has worked with this platform since launch and documentation support from ASUS.

![After run](https://cdn.osuoverclocking.com/spicer_fugger/post_run.webp)
![W9](https://cdn.osuoverclocking.com/spicer_fugger/w9_3495x.webp)

# Conclusion

This trip from Spicer and Fugger has really helped us with cleaning up some faults in our processes, and similarly to the Elmor and Scatterbencher visit, general members get to work with some of the best in the world at XOC and meet a long time community member going back to when this all began. So we all here at Oregon State Overclocking thank you for your time and willingness to educate and teach.

