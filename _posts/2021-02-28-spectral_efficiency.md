---
title: Spectral Efficiency
category: 5G
tags: 
feature_text: <h2 class="whitetext highlighted">Spectral Efficiency</h2><span class="whitetext highlighted">spectral efficiency</span> 
image: "https://images.unsplash.com/photo-1518134114050-1b126d2e81eb?ixid=MXwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHw%3D&ixlib=rb-1.2.1&auto=format&fit=crop&w=1350&q=80"
comments: true
---

This report consists in a compound of resources on analyzing 5G network from a spectral efficiency perspective. I wrapped up in this report all the useful, simple and updated information that I found on this topic across the Internet. I referenced all the resources that helped me to have a better understanding on spectral efficiency on mobile networks without not knowing so much in the topic before.

## What is Spectral Efficiency?

Spectral efficiency has to do with the amount of information that fits in a given channel bandwidth. One can say how efficiently a piece of spectrum can be used to transmit information.

It is expressed in terms of bits/sec/Hz.

TODO equation

### Shannon’s Limit

The Shannon capacity theorem bounds the rate that information can be transmitted across a noisy channel. It has the following expression:

TODO shannons eq

Where as it can be seen, the capacity is constrained by the bandwith of the channel and the signal level. To extend this section a little bit, this professor in the video below, explains in what Shannon’s boundary consists in a very simple and understandable way.

{% include video.html id="ancDN11C2vg" %}


## 5G Radio Engineering Techniques

### MIMO

High level-insight video: 

{% include video.html id="9RlM-aBbUBc" %}

5G also relies on another technology called [Massive Multiple Input Multiple Output](https://www.mwrf.com/systems/defining-massive-mimo-5g-world) (Massive MIMO). Simply put, Massive MIMO allows the transmitting and receiving of more than one data signal simultaneously over the same radio channel. To enable this, the Massive MIMO system will have many more antennas than standard MIMO networks tend to use (about two to four). While there’s no “official” figure for what constitutes a Massive MIMO, we’re talking about dozens if not hundreds of antennas here, deployed onto cell towers, utility poles, lampposts, buildings, and other public and private structures. Naturally, the more antennas a transmitter or a receiver is equipped with, the more possible signal paths there are, and the better the performance to be expected. In addition, the greater number of antennas means the Massive MIMO network will be far more resistant to interference and jams than current systems, which only use a handful of antennas.

{% include figure.html image="/assets/img/spectral_efficiency/mimo_comparison.jpeg" caption="Source: ni.com/" %}

Massive MIMO networks will also use beamforming technology. Beamforming is essentially a traffic-signaling system for cellular base stations that identifies the most efficient data-delivery route to a particular user, while reducing interference for other nearby users in the process

A deep dive in MIMO can be found [here](https://www.ni.com/es-es/innovations/white-papers/14/5g-massive-mimo-testbed--from-theory-to-reality--.html).

## Available Spectrum

5G-NR utilizes much higher radio frequencies (28 GHz compared to just 700-2,500 MHz for 4G) to transfer much more data over the air faster with reduced congestion and lower latency. The advantage of higher radio frequencies is that they are able to support much higher signal bandwidths – hence higher data throughput rates.

{% include figure.html image="/assets/img/spectral_efficiency/spectrum_5g_usa.jpg" caption="Source: https://www.qualcomm.com/news/onq/2017/10/04/path-opening-more-spectrum-5g-us" %}

### OFDM

In order to gain some high-level insights on OFDM, here there is a nice explanation: [https://www.youtube.com/watch?v=KCHO7zlU25Q](https://www.youtube.com/watch?v=KCHO7zlU25Q).

{% include video.html id="KCHO7zlU25Q" %}

Mobile wireless systems employ OFDM to achieve high bandwidth channels. Existing 4G (LTE) mobile wireless uses OFDM for the downlink (base station to mobile device), with a fixed subcarrier spacing of 15 kHz. The modulation on the subcarriers can be QPSK, 16QAM or 64QAM.

The 5G New Radio (NR) standard uses OFDM on both the uplink and downlink. The NR specification is designed with a high degree of flexibility to cover a diverse set of applications. The carrier spacing is flexible (15 kHz, 30 kHz, 60 kHz, 120 kHz, 240 kHz, 480 kHz) with up to 3300 subcarriers. The subcarrier modulation can be QPSK, 16QAM, 64QAM or 256QAM.

A deep dive on OFDM can be found [here](https://www.5gtechnologyworld.com/the-basics-of-5gs-modulation-ofdm/)

## Spectral Efficiency in 5G

A More deep and formal explanation can be found in [this paper](https://ieeexplore.ieee.org/abstract/document/7944631), where it’s proved the performance of three key 5G technologies in the sense of spectral efficiency improvement: <span style="text-decoration:underline;">sparse code multiple access</span>, <span style="text-decoration:underline;">polar codes</span>, and <span style="text-decoration:underline;">filtered orthogonal frequency-division multiplexing,</span> which are novel multiple access technology, channel coding scheme, and waveform, respectively. According to the field test results, they achieve over 100% spectral efficiency improvement in comparison with baseline, where orthogonal frequency-division multiple access and turbo coding as LTE are used.

## Comparison with 4G - 5G

Below are shown the ITU objectives for IMT‐2020:

{% include figure.html image="/assets/img/spectral_efficiency/spectral_ef_itu_2020.png" caption="" %}

Here, there is a link to a comparison table of predicted spectral efficiency values of some common communication systems:

[https://en.wikipedia.org/wiki/Spectral_efficiency](https://en.wikipedia.org/wiki/Spectral_efficiency).

## References

* [5G vs 4G in a nutshell](https://itchronicles.com/mobile/5g-vs-4g-how-mobile-networks-are-changing-forever/)

* [How to Calculate Spectral Efficiency for 5G networks ?](https://www.youtube.com/watch?v=qVXOYgczcHw)

* [5G Massive MIMO Testbed: From Theory to Reality](https://www.ni.com/es-es/innovations/white-papers/14/5g-massive-mimo-testbed--from-theory-to-reality--.html)

* [5G New Radio: The technical background](https://www.zdnet.com/article/5g-new-radio-the-technical-background/)