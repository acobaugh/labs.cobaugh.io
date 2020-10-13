+++
title = "Model 82D"
[menu.main]
identifier = "82D"
parent = "tesla"
weight = 10
+++

{{< imgproc "images/IMG_20200825_170846.jpg" Resize "x400" "" "link" >}}

## Specs

* Secondary: 8.4" x 45" winding length, 26AWG wire
* Resonant frequency: 41.3kHz
* Topload: [10" x 47" ring type](../10x47-ring-toroid)
* Primary: ~9T of 3/8" soft copper tubing, 3/8" edge-edge spacing, water cooled
* Primary Capacitor: 5s20p CDE942C20P15K MMC, 0.60uF @10KVDC, 270A RMS, 8640A peak
* Bridge
  * Layout: H-bridge with voltage doubler for 680VDC with 240VAC input
  * IGBT: 2x Mitsubishi CM300DY-24H
  * Bus capacitor: 5500uF @ 900VDC. 2x CDE 520C 11000uF, 450VDC inverter-grade electrolytic in series. 15kOhm / 10W bleeder/balance resistors
  * Bus: Laminated, 1/16" aluminum, 1/16" G10/FR4 insulating layer
  * Snubber: 2x Aerovox RBPS direct-mount, 2uF 1000VDC each
* Power Supply: [Remote single-phase 240VAC voltage doubler with precharge/discharge. 680VDC @ 20A output](../12kw-voltage-doubler)
* Driver: UD2.7C
* Feedback/OCD: 50:20:1 current transformers, Fair-rite Type 77 (5977003801 and 5977006401)
* Interrupter: [Dual Channel MIDI Interrupter](../interrupter)
* OCD: 1200A minimum
* Arc length: TBD

## Introduction

After the success of [model 81D](../81D), I decided to design a new 8" coil with more optimal physical parameters to give a much lower resonant frequency, which would allow a much higher OCD setting.

This new system would revolve around another 8" secondary, but wound with thinner wire and for 11" more than [81D](../81D). All other components are sized to match the secondary and planned arc length.

## Design

### Power Supply

[Remote 680VDC voltage doubling rectifier with builtin EMI protection.](../12kw-voltage-doubler)

### Bridge

Same as [81D](../81D#bridge), but without the onboard rectifier/doubler configuration. In addition, new PCBs were used for the gate connections.

A second version of the CM300 Gate boards was later designed, but v0.1.0 worked well enough with minimal shoot-through and ringing that this is what is on the bridge today. 820mOhm resistors were added in series with the anti-parallel Schottkey diodes to slow down the turn-off just slightly, and a lower voltage TVS diode was used to clamp the over/undershoots. The result is better than the original configuration which proved effective, so I'm running with it.

KiCad files are available on github. PRs welcome: [github.com/acobaugh/cm300dy-24h-gate-drive-board](https://github.com/acobaugh/cm300dy-24h-gate-drive-board)

{{< imgproc "images/20191228-234615.jpg" Resize "400x" "" "link" >}}
{{< imgproc "images/cm300-board.jpg" Resize "400x" "" "link" >}}
{{< imgproc "images/20200118-135132700.jpg" Resize "400x" "" "link" >}}
{{< imgproc "images/20200118-135223200.jpg" Resize "400x" "" "link" >}}
{{< imgproc "images/20200118-135339300.jpg" Resize "400x" "" "link" >}}
{{< imgproc "images/IMG_20200118_141640.jpg" Resize "400x" "" "link" >}}

{{< clear >}}

### Driver

Same as [81D](../81D#driver), but with a simple 555 add-on board to allow the signal LED to glow brighter.

{{< clear>}}

### Primary

9 turns 3/8" copper with water cooling.

{{< imgproc "images/IMG_20200806_202441.jpg" Resize "400x" "" "link" >}}
{{< imgproc "images/IMG_20200829_195901.jpg" Resize "400x" "" "link" >}}
{{< imgproc "images/IMG_20200906_163207.jpg" Resize "400x" "" "link" >}}
{{< imgproc "images/IMG_20200906_163219.jpg" Resize "400x" "" "link" >}}

### Secondary

The secondary is a piece of 8" SDR-35 drain pipe that has been sanded, sealed with polyurethane, wound, then coated with Envirotex Lite 2-part epoxy for a protective, glass-like finish. The ends are finished the same as 81D, with 1/2" pieces of HDPE secured with nylon screws along the edge. The mount is a 1/2-13 nut captured in machined blocks of HDPE on the inside. 

Ground connection is a piece of 5/8"x1/16" copper bent to follow the curvature of the pipe and a piece of brass soldered to it, which is then drilled and tapped for a screw.

{{< imgproc "images/IMG_20191028_210734.jpg" Resize "400x" "" "link" >}}
{{< imgproc "images/IMG_20191019_161511.jpg" Resize "400x" "" "link" >}}
{{< imgproc "images/IMG_20191022_134936.jpg" Resize "400x" "" "link" >}}
{{< imgproc "images/20191109-143321200.jpg" Resize "400x" "" "link" >}}
{{< imgproc "images/20191109-143504700_half.jpg" Resize "400x" "" "link" >}}
{{< imgproc "images/IMG_20191127_165809.jpg" Resize "400x" "" "link" >}}
{{< imgproc "images/IMG_20191203_205856.jpg" Resize "400x" "" "link" >}}
{{< imgproc "images/IMG_20191203_212138.jpg" Resize "400x" "" "link" >}}
{{< imgproc "images/IMG_20191205_201816.jpg" Resize "400x" "" "link" >}}
{{< imgproc "images/IMG_20191205_225203.jpg" Resize "400x" "" "link" >}}
{{< imgproc "images/IMG_20191205_230250.jpg" Resize "400x" "" "link" >}}
{{< imgproc "images/IMG_20191206_200955.jpg" Resize "400x" "" "link" >}}
{{< imgproc "images/IMG_20200906_181858.jpg" Resize "400x" "" "link" >}}
{{< clear >}}

{{< youtube "RV8_y-cIPhU" >}}

### Base

{{< imgproc "images/IMG_20200906_164250.jpg" Resize "400x" "" "link" >}}
{{< imgproc "images/PXL_20201003_002653642.jpg" Resize "400x" "" "link" >}}
{{< imgproc "images/PXL_20200916_000948490.jpg" Resize "400x" "" "link" >}}
{{< imgproc "images/PXL_20200916_000952563.jpg" Resize "400x" "" "link" >}}
{{< imgproc "images/PXL_20200915_233735293.jpg" Resize "400x" "" "link" >}}
{{< imgproc "images/IMG_20200827_210443.jpg" Resize "400x" "" "link" >}}
{{< imgproc "images/IMG_20200827_210511.jpg" Resize "400x" "" "link" >}}

{{< clear >}}

### Tuning

### Videos
