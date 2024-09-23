---
layout: post
title: UAV-assisted wireless localization
author: Fraida Fund
tags: [wireless, aerpaw]
---

You've been asked to contribute your machine learning expertise to a crucial and potentially life-saving mission.

A pair of hikers has gone missing in a national park, and they are believed to be critically injured. Fortunately, they have activated a wireless locator beacon, and it transmits a constant wireless signal from their location. Unfortunately, their beacon was not able to get a satellite fix, so their GPS position is not known.

To rescue the injured hikers, therefore, their location must be estimated using the signal strength of the wireless signal from the beacon: when a radio receiver is close to the beacon, the signal strength will be high. When a radio receiver is far from the beacon, the signal strength will be lower. (The relationship is noisy, however; the wireless signal also fluctuates over time, even with a constant distance.)

You are going to fly an unmanned aerial vehicle (UAV) with a radio receiver around the area where they were last seen, and use the received wireless signal strength to fit a machine learning model that will estimate the hikers' position. Then, you'll relay this information to rescuers, who will try to reach that position by land. (Unfortunately, due to dense tree cover, the UAV will not be able to visually confirm their position.)

There is a complication, though - the UAV has a limited battery life, and therefore, limited flight time. You'll have to get an accurate estimate of the hikers' position in a very short time!

[UAV-assisted wireless localization](https://colab.research.google.com/github/teaching-on-testbeds/uav-wireless-localization/blob/main/8_kernel_find_a_rover.ipynb)
