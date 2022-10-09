# Lab 4: Building a Channel Sounder

A channel sounder is a device that measures the channel response between
a transmitter (TX) and receiver (RX).  Channel sounders are key for researchers
studying wireless channel propagation.
They are also useful in bringing up any SDR platform to ensure the wideband
response through the TX and RX chains is as expected.
Indeed,  after ensuring you can receive a tone correctly, use a channel sounder
to make sure the device works and correctly characterize the TX and RX filters.

In going through this lab, you will learn to:
* Measure the channel frequency response via frequency-domain correlation
* Compute the time-domain channel impulse response via an IFFT
* Align the channel impulse response via peak detection
* Estimate the SNR
* Build a continuous monitor for the channel  

<img src="chanSounder.gif" alt="Estimated channel taps over time" width="350">

## Files:

* The main file is `chanSounder.mlx`:  [[Matlab]](./chanSounder.mlx) [[PDF]](./chanSounder.pdf).
* The file `estChanResp.m` is a function for computing the estimated channel.

For the lab, complete the `TODO` sections in both files, run `chanSounder.mlx`,
and print to PDF.  Submit the PDF.
