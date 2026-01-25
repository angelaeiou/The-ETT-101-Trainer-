# The Emona Telecoms-Trainer 101 👾
This repository contains a collection of laboratory experiments for ETT 101 using the Emona Telecommunications Trainer. It is designed to help students understand fundamental communication and telecommunications principles through hands-on activities, practical measurements, and signal analysis.

## Table of Contents 📚
* [Part 1: Oscilloscope Setup and Signal Measurement](#-part-1-oscilloscope-setup-and-signal-measurement)

* [Part 2: Introduction to the Emona Telecommunications Trainer 101](#-part-2-introduction-to-the-emona-telecommunications-trainer-101)
  * [Part 2.1: Master Signals, Speech, and Buffer Module](#-part-21-master-signals-speech-and-buffer-module)
  * [Part 2.2: Adder and Phase Shifter Module](#-part-22-adder-and-phase-shifter-module)
  * [Part 2.3: Voltage-Controlled Oscillator (VCO) Module](#-part-23-voltage-controlled-oscillator-vco-module)
  
* [Part 3: Mathematical Equation Modeling Using the ETT 101](#-part-3-mathematical-equation-modeling-using-the-ett-101)

* [Part 4: Amplitude Modulation (AM)](#-part-4-amplitude-modulation-am)
  
# Part 1: Oscilloscope Setup and Signal Measurement 〰️

## Abstract
This experiment focused on the proper setup and operation of a dual-channel 20 MHz analog oscilloscope. The objective was to familiarize the user with essential oscilloscope controls required to obtain a stable and accurate waveform display. Through systematic configuration of the general, vertical, horizontal, and triggering controls, a stable AC signal was successfully observed. The experiment reinforces fundamental concepts such as amplitude, period, and frequency, which are critical for accurate signal measurement in electronics laboratories.
### Introduction
The oscilloscope is one of the most versatile and widely used instruments in electronics and communication engineering. It provides a visual representation of electrical signals by displaying voltage as a function of time. Proper oscilloscope setup is essential, as incorrect control settings can result in unstable waveforms or inaccurate measurements.
### Theoretical Background
An oscilloscope displays electrical signals in the time domain. The *amplitude* of a signal refers to its physical size and is measured in volts (V), commonly as peak or peak-to-peak voltage. The *period* is the time required for one complete cycle of a waveform and is measured in seconds (s). The *frequency* is the number of cycles per second and is measured in hertz (Hz), where frequency is the reciprocal of the period.

A *sine wave* is a smooth, continuous periodic waveform commonly used to represent AC signals. A *square wave* is a periodic signal that alternates between two discrete voltage levels and is often used in digital and timing applications.

### Experimental Results 
<details>
  <summary><strong>Waveform Output</strong></summary>

  <p align="center">
    <img src="Results/laboratory results 1/data_waveform1.jpg" alt="Waveform Output" width="600">
  </p>
   <p align="center">
<em>
     Figure 1.1.1: Square-wave output from the internal CAL source at 1 kHz, corresponding to a 1 ms time period.
   </em> 
   </p>
   <p align="center">
    <img src="Results/laboratory results 1/data_waveform2.jpg" alt="Waveform Output" width="600">
  </p>
  <p align="center">
<em>
     Figure 1.1.2: Square-wave signal displayed measured at approximately 2 V/div with a time base of 500 µs/div. The waveform shows a periodic signal with a frequency around 1 kHz.
   </em> 
     </p>
</details>

# Part 2: Introduction to the Emona Telecommunications Trainer 101 👩🏻‍💻

## Abstract

This experiment focused on exploring and understanding the operation of the Emona Telecoms-Trainer 101 modules. The objective was to familiarize the user with the Master Signals, Speech, Buffer, Adder, Phase Shifter, and Voltage-Controlled Oscillator (VCO) modules. By systematically connecting and observing the behavior of each module, fundamental principles of communications and signal processing were demonstrated. The experiment reinforces critical concepts such as signal summation, phase shifting, modulation, and voltage-controlled oscillation, which are essential in telecommunications systems.
 <p align="center">
    <img src="Results/laboratory results 1/emona telecoms.jpg" alt="Waveform Output" width="600">
  </p>

### Introduction

This repository contains documentation and explanations for the Telecoms-Trainer 101 modules used in telecommunications experiments. It covers the operation, theoretical background, and practical usage of:

- Master Signals Module
- Speech Module
- Buffer Module
- Adder Module
- Phase Shifter Module
- Voltage-Controlled Oscillator (VCO) Module

### Part 2.1: Master Signals, Speech, and Buffer Module

The Master Signals, Speech, and Buffer modules provide the primary sources of audio and analog signals in the Telecoms-Trainer 101 system. The Master Signals module generates reference signals, while the Speech module introduces human voice signals for processing. The Buffer module ensures proper signal isolation, preventing interference between modules while maintaining signal integrity.

#### The Master Signal Module 

Master Signals Module

The Master Signals module produces stable, predictable waveforms such as:

Sine waves – smooth periodic oscillations used for frequency response testing.

Square waves – useful for digital signal testing and timing analysis.

Triangular waves – commonly used in modulation and waveform analysis.

These waveforms serve as input signals for testing circuits, helping users study how systems respond to different signal types. Connecting the module to an oscilloscope allows observation of amplitude, frequency, and waveform shape.
<details>
  <summary><strong>Master Signal Block Diagram</strong></summary>

 <p align="center">
    <img src="Results/laboratory files 2/Setups/Master Signals Block Diagram.jpeg" alt="Waveform Output" width="600">
  </p>
<p align="center">
  <em>Figure 2.1.1: Master Signal Block Diagram</em>
</p>

<p align="center">
    <img src="Results/laboratory files 2/Setups/Master Signal Setup.jpeg" alt="Waveform Output" width="600">
  </p>
<p align="center">
  <em>Figure 2.1.2: Master Signal Basic Setup</em>
</p>
   <p align="center">
    <img src="Results/laboratory files 2/Setups/Master Signal Setup SinCos.jpeg" alt="Waveform Output" width="600">
  </p>
<p align="center">
  <em>Figure 2.1.3: Master Signal with Sin Cos Representation</em>
</p>

### Results 
 <p align="center">
    <img src="Results/laboratory files 2/Results/Master Signals SinCos.jpeg" alt="Waveform Output" width="600">
  </p>
<p align="center">
  <em>Figure 2.1.3: Master Signal with Sin Cos Representation in Oscilloscope</em>
</p>

The oscilloscope displays the sine and cosine outputs from the Master Signals module set at 100 kHz. Both waveforms have the same frequency and amplitude but exhibit a phase difference of approximately 90°, which is characteristic of sine and cosine signals. This result confirms the proper operation of the Master Signals module in generating quadrature signals for signal analysis and communication applications.

</details>





