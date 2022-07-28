# Photoplethysmogram Biosignal Detector
Designing and wiring an analog circuit for a photoplethysmogram to detect blood volume changes for biosignal indicators.

## Description

This analog circuit uses the general block diagram below to measure biosignals using your finger. A phototransistor acts as a sensor by adjusting current based on the light that is able to pass through your finger. This light level varies with blood volume, which can make the corresponding current indicative of biosignals. This signal is then passed through a cascaded fitler, gain circuit, and comparator before being fed into an LED to visualize the biosignal. 

<img width="548" alt="image" src="https://user-images.githubusercontent.com/43231577/181640330-d0b417bd-69bf-4207-b1b5-aaae400c11aa.png">

## Getting Started

<img width="285" alt="image" src="https://user-images.githubusercontent.com/43231577/181636013-a3afe355-fde8-4075-b474-b82a5f8b6860.png">

### Dependencies

* 1 TCRT1010 reflective optical sensor
* 5 LM741 transistors 
* Resistors:
  * 1 330 $\Omega$
  * 2 10K $\Omega$
  * 1 2.2K $\Omega$
  * 1 45.1K $\Omega$
  * 1 134K $\Omega$
  * 1 142.8K $\Omega$
  * 1 7.8K $\Omega$
  * 1 8.2K $\Omega$
  * 2 1K $\Omega$
  * 1 100 $\Omega$
  * 1 220K $\Omega$
* Capacitors
  * 2 10 $\mu F$
  * 1 1 $\mu F$
  * 1 0.1 $\mu F$

### Installing

* Download all files into a local directory in order to later upload to the respective Arduino boards.

### Executing program

* =

## Authors
* Bhushan Patel
* Billy Beauregard

## Acknowledgments
* Harvard Active Learning Labs staff
