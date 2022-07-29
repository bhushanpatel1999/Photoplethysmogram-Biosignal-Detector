# Photoplethysmogram Biosignal Detector
Designing and wiring an analog circuit for a photoplethysmogram to detect blood volume changes for biosignal indicators.

## Description

This analog circuit uses the general block diagram below to measure biosignals using your finger. A phototransistor acts as a sensor by adjusting current based on the light that is able to pass through your finger. This light level varies with blood volume, which can make the corresponding current indicative of biosignals. This signal is then passed through a cascaded fitler, gain circuit, and comparator before being fed into an LED to visualize the biosignal. 

<img width="548" alt="image" src="https://user-images.githubusercontent.com/43231577/181640330-d0b417bd-69bf-4207-b1b5-aaae400c11aa.png">

## Getting Started

### Specifications

* The bandwidth of 0.5 - 5 Hz should be preserved,
* Peak-to-peak amplitude at the output should exceed 3.5V,
* All active filters should conform to the Sallen-Key topology,
* Less than 5% composite gain distortion in the final passband (theoretical),
* Less than 100 mV mean DC offset at steady state,
* Less than 10 seconds settling time for offset perturbation,
* The entire system should be powered by a 9V battery,
* Theoretical battery life and SNR should be reasonably maximized.

NOTE: The design process of the filters and the corresponding waveforms can be found inside the Jupyter Notebook file.

Below is the circuit diagram for the detector implementing these specifications:

<img width="285" alt="image" src="https://user-images.githubusercontent.com/43231577/181636013-a3afe355-fde8-4075-b474-b82a5f8b6860.png">

### Dependencies (hardware and software)

* 9V power supply
* 1 TCRT1010 reflective optical sensor
* 5 LM741 op-amps 
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
* Red LED
* Digilent Analog Discovery Studio (optional)
* Digilent Waveforms desktop application (optional)

### Executing circuit

Because this is an analog circuit, nothing more than a breadboard, power supply, ground, and the listed components is needed. The LED is one way to verify the working of your circuit. However, while optional, the circuit can also be built using Digilent's Analog Discovery Studio and the individual analog signals verified using the accompanying Waveforms application. 

## Authors
* Bhushan Patel
* Kyle Fullen

## Acknowledgments
* ENG-SCI 152: Circuits, Devices, and Transduction staff
