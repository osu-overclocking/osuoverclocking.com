---
title: 'A Visit From Fugger and Spicer'
date: 2025-12-03T12:40:44-08:00
draft: false
tags: [Visit]
author: "Zander Ray"
featured_image: "https://cdn.osuoverclocking.com/spicer_fugger/Group_shot.webp"
description: "Collaborative Evaluation of Modern CPU Architectures with Established XOC Community Members: Report"
---

# Goals

With this collaboration, the primary objective was to acquire platform-specific knowledge and best practices that could be integrated into our own extreme overclocking (XOC) workflows. This was accomplished through hands-on benching sessions led by Charles Wirth (Fugger) and Max Spicer (Spicer), who traveled to work directly with our members on several shared platforms. The architectures evaluated during this session were Arrow Lake (Intel), AM5 (AMD), and Sapphire Rapids / W790 (Intel).

---

# Memory Overclocking

![Spicer Teaching](https://cdn.osuoverclocking.com/spicer_fugger/spicer_w_member.webp)

The Arrow Lake platform was primarily evaluated through memory frequency validation (Mem Valid), a benchmark category that emphasizes raw memory frequency stability and signal integrity rather than full system throughput. As of writing, the global record for this category stands at 6765.2 MHz (memory clock).

It is worth clarifying that consumer memory kits are typically marketed using megatransfers per second (MT/s), which is twice the actual operating frequency due to DDR (Double Data Rate) signaling. For example, a “6400 MT/s” kit operates at a true clock frequency of 3200 MHz.

Arrow Lake demonstrated several architectural traits that make it well-suited for memory frequency scaling:

* A strong integrated memory controller (IMC) with favorable cold behavior

* Fine-grained memory training controls

* Robust signal integrity on high-end Z890 motherboards

Working alongside Spicer, we achieved a validated frequency of 5512.8 MHz on an ASUS ROG Z890 Apex motherboard paired with an Intel Core Ultra 7 265K, using liquid nitrogen (LN2) cooling. This session emphasized IMC tuning, training retries, and temperature-dependent stability windows.

To support this process, a variety of tools from Elmor Labs were used, including the Hot300 heater, heater plate, Volcano LN2 pot, and OC Panel. These tools significantly improved repeatability and accessibility during the session. For example, the OC Panel’s large POST code display proved especially valuable during cold training cycles, particularly for members with limited visibility near the bench table.

# AM5 Overclocking

![7950x setup](https://cdn.osuoverclocking.com/spicer_fugger/Am5.webp)

The AMD AM5 platform was explored due to its strong competitiveness in global ranking systems, particularly in benchmarks that favor higher core counts and efficient multi-thread scaling. From an architectural standpoint, AM5 presents a comparatively constrained but predictable overclocking environment.

* Key architectural observations included:

* Limited core frequency headroom relative to Intel platforms

* Heavy reliance on Precision Boost and voltage scaling behavior

* Strong memory and fabric coupling effects

One notable behavior observed on the Ryzen 9 7950X was the interaction between SoC-related voltage rails and cold bug characteristics. By adjusting these rails, we were able to entirely remove the cold bug, allowing the processor to operate at full LN2 pot temperatures. However, this came at the cost of approximately 2% performance degradation, indicating internal trade-offs between cold tolerance and execution efficiency.

AM5’s dual-CCD topology introduced additional tuning considerations. With guidance from Spicer, we examined CCD balancing and Infinity Fabric (FCLK) optimization in greater depth. While FCLK tuning has long been known to affect performance, new insight into feed voltages and stability thresholds has improved our ability to push fabric clocks more aggressively without destabilizing the system.

Overall, AM5 proved to be a technically clean platform with fewer variables than Arrow Lake, making it approachable for newer members while still offering depth through memory and fabric optimization.

# Modern HEDT

![Setup of w9](https://cdn.osuoverclocking.com/spicer_fugger/pre_run.webp)

Modern HEDT remains one of the most technically demanding segments of the desktop CPU landscape. While Intel’s X299 platform and the 10980XE represented the last traditional HEDT generation, the Xeon W9-3495X introduces a dramatically different class of challenges.

This processor features 56 cores and 112 threads, is fully multiplier unlocked, and exhibits extreme power density under load. In our testing, sustained power draw exceeded 2000 W, fundamentally shifting the limiting factor from frequency scaling to thermal transport and system-level power delivery.

* Architectural characteristics of note included:

* A cold bug window around –50 °C to –60 °C, leaving minimal temperature headroom

* Extremely high heat flux due to dense core layout

* Strong scaling in AI and throughput-focused workloads

Because of these constraints, cooling efficiency became paramount. We employed an Elmor Labs Volcano X LN2 pot to maximize heat transfer efficiency, along with a dedicated LN2 refill workflow to maintain consistent thermal conditions. Power delivery was handled by two 2200 W PSUs, ensuring sufficient overhead for transient loads.

Using an ASUS Pro WS W790E-SAGE SE motherboard, and with platform-specific guidance from Fugger—who has extensive experience with W790 since launch—we achieved the highest Geekbench AI score on this platform as of writing. ASUS-provided documentation and firmware support played a critical role in enabling this result.
![After run](https://cdn.osuoverclocking.com/spicer_fugger/post_run.webp)
![W9](https://cdn.osuoverclocking.com/spicer_fugger/w9_3495x.webp)

# Conclusion

This collaborative session with Spicer and Fugger provided substantial value by refining our understanding of modern CPU architectures under extreme operating conditions. Each platform—Arrow Lake, AM5, and W790—presented distinct architectural strengths and constraints, reinforcing the importance of platform-specific methodologies rather than one-size-fits-all approaches.

Beyond benchmark results, the most significant outcome was the improvement of our internal processes, documentation, and teaching workflows. Similar to prior visits from Elmor and ScatterBencher, this event allowed general members to work directly with world-class XOC practitioners and engage with long-standing contributors to the overclocking community.

On behalf of Oregon State Overclocking, we sincerely thank Spicer and Fugger for their time, expertise, and willingness to educate the next generation of extreme overclockers.