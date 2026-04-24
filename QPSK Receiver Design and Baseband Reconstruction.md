This repository presents the laboratory implementation of a **Quadrature Phase Shift Keying (QPSK) communication receiver**, focusing on the extraction of baseband information from a phase-modulated carrier. The project demonstrates how digital information can be transmitted efficiently by encoding data into carrier phase changes and later reconstructed through coherent demodulation.

---

## Repository Contents

- [Introduction](#introduction)
- [Theory of Operation](#theory-of-operation)
- [Transmitter Section](#transmitter-section)
- [Channel Simulation](#channel-simulation)
- [Receiver Section](#receiver-section)
- [Noise Investigation](#noise-investigation)
- [Experimental Images](#experimental-images)
- [Signal Analysis](#signal-analysis)
- [Conclusion](#conclusion)

---

## Introduction

Quadrature Phase Shift Keying (**QPSK**) is a digital modulation technique that allows a carrier signal to represent **two binary bits per symbol**. Instead of transmitting one bit at a time, QPSK maps pairs of bits into four possible carrier phase states:

- 45°
- 135°
- 225°
- 315°

Because two bits are carried in each symbol, QPSK improves spectral efficiency compared to conventional binary phase modulation systems.

---

## Theory of Operation

The QPSK waveform is represented by:

\[
s(t)=I(t)\cos(2\pi f_ct)+Q(t)\sin(2\pi f_ct)
\]

Where:

- `I(t)` = in-phase data  
- `Q(t)` = quadrature data  
- `fc` = carrier frequency  

The receiver separately recovers both components and reconstructs the original serial information.

---

## Transmitter Section

The transmitter was divided into three main blocks.

### Data Splitting
The binary input stream was divided into:
- Even bits → I channel  
- Odd bits → Q channel  

### Orthogonal Modulation
Each channel modulated an orthogonal carrier:
- I channel → cosine carrier  
- Q channel → sine carrier  

### Signal Combination
The two modulated outputs were summed to create the QPSK signal.

### Transmitter Block Diagram

<img src="images/qpsk_tx.png" width="700">

---

## Channel Simulation

To simulate practical transmission, the signal passed through a channel model that introduced:

- attenuation  
- phase shift  
- additive noise  

### Channel Model

<img src="images/channel_model.png" width="700">

---

## Receiver Section

The receiver performed coherent demodulation using several stages.

### Carrier Recovery
A synchronized oscillator generated:
- cosine reference  
- sine reference  

### Product Detection
The received signal was multiplied with:
- cosine for I recovery  
- sine for Q recovery  

### Low-Pass Filtering
Each output was filtered to remove unwanted high-frequency components.

### Serial Reconstruction
Recovered parallel bits were recombined into the original bit stream.

### Receiver Block Diagram

<img src="images/qpsk_rx.png" width="700">

---

## Noise Investigation

Noise was gradually added to observe system behavior.

### Observations

- Low noise → accurate recovery  
- Medium noise → waveform distortion  
- High noise → symbol errors  

### Noise Effect

<img src="images/noise_signal.png" width="700">

---

## Experimental Images

### Modulated Signal

<img src="images/modulated_waveform.jpg" width="700">

### Recovered Output

<img src="images/recovered_data.jpg" width="700">

---

## Signal Analysis

The experiment verified that:

- QPSK transmits two bits per symbol
- Orthogonal carriers prevent interference
- Coherent detection restores the original data
- Noise increases decision errors

The recovered output closely matched the transmitted signal under low-noise conditions.

---

## Conclusion

The laboratory successfully demonstrated the implementation of a complete QPSK receiver system. The experiment showed how orthogonal carrier components can be separated, filtered, and recombined to recover the original digital message.

---

