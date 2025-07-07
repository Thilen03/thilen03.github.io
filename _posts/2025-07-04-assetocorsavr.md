---
layout: post
title: How I Improved VR Visuals and Performance in Assetto Corsa
date: 2025-07-04 16:42
category: [Sim Racing] 
author: 
tags: [Modding]
summary: 
---
![Image](https://www.roadtovr.com/wp-content/uploads/2017/03/assetto-corsa-vr.jpg)
I recently got into Assetto Corsa in VR and after a few days of research I found the best options that worked for me. I was having issues with flickering, weird shadow rendering, and texture artifacts. Even with decent performance and resolution, the visuals didn’t look right. After testing different settings and mods I finally got sharp visuals and stable performance. I want to share this to help others with similar problems.

I switched from SteamVR to OpenComposite combined with OpenXR. This gave me a bit more FPS, but more importantly it greatly improved the consistency of my frametimes, which made the experience smoother and more comfortable. OpenComposite replaces SteamVR for supported games and redirects them to OpenXR. You can find it here: [OpenOVR](https://gitlab.com/znixian/OpenOVR). The page also has info on tuning the opencomposite.ini file, which lets you adjust many parameters to fit your hardware and preferences.

I then installed Custom Shaders Patch 0.2.12p1, the only build currently supporting Snowymoon’s TAA mod in VR. This version is available on Patreon. I also use Pure mod version 2.57 along with the 2.60 hotfix, which is required for Pure and the TAA mod to work properly together. Using TAA fixed most artifacts on textured objects like flickering shadows and shimmering edges. Overall, Snowymoon’s TAA is a game changer, whether you use a graphics mod or not. It’s bloody brilliant and really cleans up the visuals. With Pure and TAA combined, the image became much clearer and more stable during movement. I have not tested the alternative SOL mod so I can’t comment on that.

Snowymoon’s mod is free, and all CSP-specific settings you need to change for it are listed on their website: [Snowymoon.io](https://snowymoon.io/).

For OpenXR I used CAS at 70% sharpness to improve image clarity without oversharpening. Other settings were mostly personal preference. You can also supersample your headset from here if you want even greater clarity, this will nuke your fps though. I haven’t tested FSR but from what Snowymoon said it breaks TAA, so I never bothered to try it out.

In Content Manager I left most settings the same, except for disabling MSAA (which conflicts with TAA and causes artifacts) and reducing particle effects, which I don’t find necessary in VR. It depends on what your system can handle.

My system specs for reference: CPU: AMD Ryzen 5 5800X3D GPU: AMD Radeon RX 6900 XT RAM: 32 GB VR Headset: Pico, 2160x2160
