# Software Defined Radio labs

[Sundeep Rangan](https://wireless.engineering.nyu.edu/sundeep-rangan/), Professor, ECE, New York University

This repo contains some simple labs for software defined radios (SDRs).  I am developing these to be used in conjunction
with the undergraduate and graduate digital communications classes at New York University.  The initial labs are based on
the simple [ADALM-Pluto boards](https://www.analog.com/en/design-center/evaluation-hardware-and-software/evaluation-boards-kits/adalm-pluto.html)
from Analog Devices. In these labs, I will use the simple [MATLAB interface](https://www.mathworks.com/help/supportpkg/plutoradio/ug/install-support-package-for-pluto-radio.html).  NYU students enrolled in the class will be able to borrow a Pluto device from the instructor.  All NYU students also have free access to MATLAB.

<img src="ADALM-Pluto-web.png" alt="ADALM Pluto" width="300">

## Overview
All labs require one or two Pluto devices and one or two host computers.  Windows, MAC, or Linux should be fine, but I have only tried Windows so far.
I am hoping to make most labs runs in one of three modes:
* *Loopback* where a single Pluto is connected to a single PC and you TX and RX from the same device.  This is the simplest, but obviously results in uninteresting channels.
* *Two devices, single host* where two Pluto devices are connected to the same host.  One is used for TX and the second for RX.  This allows somewhat more interesting channels, but you can only separate the devices by the length of the cables from the host PC.
* *Two devices, two hosts* where two Pluto devices are connected to two different hosts.  One is used for TX and the second for RX.  This allows the most realistic channels, but you will require two hosts.
NYU students enrolled in the class are provided one Pluto each.  So, the two device experiments require a partner.

In most of the initial labs, the TX will simply repeatedly transmit the identical data in a continuous loop.  The RX will capture samples and the processing will be performed offline. This method provides the full realism of a channel, but is limited to a short burst of communication.

Each lab is provided as a MATLAB Live script.  Students should download the script and fill in the sections labeled `TODO`.  NYU students in the class should fill in the `TODO` sections, print the PDF and submit the PDF.  Labs should be performed with two students.  Submit only one lab per pair.  NYU students will be provided the solutions in class.  If you are instructor and interested in the solutions, please write me.  

## Labs

* Lab 1:  Setting up the SDR and capturing and receiving baseband samples
