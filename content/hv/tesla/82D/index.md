+++
title = "Model 82D"
[menu.main]
identifier = "82D"
parent = "tesla"
+++

## Specs

* Secondary: 8.4" x 45" winding length, 26AWG wire
* Topload: 11" x 45" ring type
* Primary: 9T of 3/8" soft copper tubing, 3/8" edge-edge spacing
* Primary Capacitor: 5s16p CDE942C20P15K MMC, 0.48uF @10KVDC, 216A RMS, 6912A peak
* Bridge
  * Layout: H-bridge with voltage doubler for 680VDC with 240VAC input
  * IGBT: 2x Mitsubishi CM300DY-24H
  * Bus capacitor: 5500uF @ 900VDC. 2x CDE 520C 11000uF, 450VDC inverter-grade electrolytic in series. 15kOhm / 10W bleeder/balance resistors
  * Bus: Laminated, 1/16" aluminum, 1/16" G10/FR4 insulating layer
  * Rectifier: Semikron semipak SKKD81/16
  * Snubber: 2x Aerovox RBPS direct-mount, 2uF 1000VDC each
* Driver: UD2.7C
* Feedback/OCD: 50:20:1 current transformers, Fair-rite Type 77 (5977003801 and 5977006401)
* Interrupter: [Dual Channel MIDI Interrupter](../interrupter)
* OCD: 1200A minimum
* Arc length: ~7ft with ~200VAC input running ~45uS on-time while playing music.

## Introduction

After the success of [model 81D](../81D), I decided to design a new 8" coil with more optimal physical parameters to give a much lower resonant frequency, which would allow a much higher OCD setting.

This new system would revolve around another 8" secondary, but wound with thinner wire and for 11" more than [81D](../81D). All other components are sized to match the secondary and planned arc length.

## Design

### Bridge

Same as [81D](../81D#bridge)

{{< clear >}}

### Driver

Same as [81D](../81D#driver)

{{< clear>}}

### Primary

### Secondary

{{< imgproc "images/IMG_20191028_210734.jpg" Resize "400x" "" "link" >}}
{{< imgproc "images/IMG_20191019_161511.jpg" Resize "400x" "" "link" >}}
{{< imgproc "images/IMG_20191022_134936.jpg" Resize "400x" "" "link" >}}
{{< imgproc "images/20191109-143321200.jpg" Resize "400x" "" "link" >}}
{{< imgproc "images/20191109-143504700_half.jpg" Resize "400x" "" "link" >}}

{{< clear >}}

{{< youtube "RV8_y-cIPhU" >}}

### Tuning

### Videos
