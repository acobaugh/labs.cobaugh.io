+++
title = "8\" DRSSTC"
[menu.main]
identifier = "8inch-drsstc"
parent = "tesla"
+++

{{< imgproc "images/IMG_20180812_153743.jpg" Resize "x400" "" "link" >}}

## Specs

* Coming soon

## Introduction

In early 2018, I was bit by the DRSSTC bug when it became apparent just how
much heavy iron I had accumulated in my quest to bring my 15kVA Pole Pig
powered SGTC online.

I already had a large heatsink salvaged from a 7kVA UPS system. I figured I
could reconfigure my existing CDE 942C MMC to get one good for 10kVDC @208A
RMS. I simply needed a driver, bus caps, interrupter, IGBTs, and a few other
odds and ends to construct the bridge.

This coil is based around a full bridge of CM300HA-24H modules, a 2x2 bus
capacitor / doubler arrangement for 6000uF @900VDC, [Gao Guangyan's UD 2.7
driver](http://www.loneoceans.com/labs/ud27/), and the same 8" secondary and
3/8" primary from the (8" SGTC")[../8inch-sgtc].

## Design

### Bridge

{{< imgproc "images/IMG_20180907_202320.jpg" Resize "400x" "left" "link" >}}
{{< imgproc "images/IMG_20180907_202630.jpg" Resize "400x" "left" "link" >}}
{{< imgproc "images/IMG_20180806_175430.jpg" Resize "400x" "left" "link" >}}
{{< imgproc "images/IMG_20180812_153720.jpg" Resize "400x" "left" "link" >}}
{{< imgproc "images/IMG_20180812_153743.jpg" Resize "400x" "left" "link" >}}
{{< imgproc "images/IMG_20180907_195030.jpg" Resize "400x" "left" "link" >}}
{{< imgproc "images/IMG_20180908_185524.jpg" Resize "400x" "left" "link" >}}
{{< imgproc "images/IMG_20180909_191919.jpg" Resize "400x" "left" "link" >}}

{{< clear >}}

### Driver

The driver is [Loneocean's UD 2.7C](http://www.loneoceans.com/labs/ud27/), with
the HFBR series ST fiber module installed.

{{< imgproc "images/IMG_20181007_134209.jpg" Resize "400x" "left" "link" >}}
{{< imgproc "images/IMG_20181007_194909.jpg" Resize "400x" "left" "link" >}}
{{< imgproc "images/IMG_20181007_194914.jpg" Resize "400x" "left" "link" >}}
{{< imgproc "images/IMG_20181008_190453.jpg" Resize "400x" "left" "link" >}}
{{< imgproc "images/IMG_20181008_190511.jpg" Resize "400x" "left" "link" >}}
{{< imgproc "images/IMG_20181007_221033.jpg" Resize "400x" "left" "link" >}}

{{< clear >}}

