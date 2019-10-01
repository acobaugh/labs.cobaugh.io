+++
title = "Dual channel MIDI Interrupter"
[menu.main]
identifier = "interrupter"
parent = "tesla"
+++

{{<imgproc "images/IMG_20190920_090843.jpg" Resize "x400" "" "link">}}

## Introduction

This is my take on Gao Guangyan's [MIDI2 interrupter](http://www.loneoceans.com/labs/sales/midi2/). It features the MIDI2 interrupter board, an Adafruit PowerBoost 1000C LiPo battery management module and 5V boost converter, USB charging, a 1S 1200C LiPo, and a custom 555-based "burst mode" add-on board.

The burst mode board is a simple astable 555 oscillator with independent on and off time, and two ranges, a high and a low. This provides bursts from 1/s up to the same rate as the interrupter itself, providing for some interresting audio effects. The 555 OUT pin simply drives a trio of 2N3904's, two of which enable or disable each channel of the interrupter, and the third drives an LED. Burst mode is disabled by flipping a switch, which disconnects the OUT pin and pulls the bases of the transistors up to V<sub>cc</sub>.

The on-board 5V regulator of the MIDI2 board is bypassed to feed 5V into it directly from the PowerBoost module.

The PowerBoost was modified to provide remote mounting of the low-battery, charging, and done LEDs.

Finally, as a brute-force fix for transients on V<sub>cc</sub> causing the ATMega microntrollers to lock up or reset when running in burst mode, a 1000uF electrolytic cap was mounted directly to the burst mode board. This also smoothed the ripple from the boost converter to <50mV.

All of this was crammed into a small aluminum box, which was then powder coated black.

## Photos

{{<imgproc "images/IMG_20190901_200033.jpg" Resize "x400" "" "link">}}
{{<imgproc "images/IMG_20190919_144714.jpg" Resize "x400" "" "link">}}
{{<imgproc "images/IMG_20190908_222929.jpg" Resize "x400" "" "link">}}
{{<imgproc "images/IMG_20190910_234709.jpg" Resize "x400" "" "link">}}
{{<imgproc "images/IMG_20190919_224842.jpg" Resize "x400" "" "link">}}
{{<imgproc "images/IMG_20190920_092338.jpg" Resize "x400" "" "link">}}
{{<imgproc "images/interrupter_burst_mode.jpg" Resize "x400" "" "link">}}


