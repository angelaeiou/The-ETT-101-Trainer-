# Bandwidth Limiting and Restoring Signals

---

### Abstract
This experiment investigated the effects of **bandwidth limitation on digital communication signals**, particularly in Pulse Code Modulation (PCM) systems. The objective was to observe how restricting the bandwidth of a transmission channel affects the quality and shape of digital signals. Through PCM decoding, waveform observation, and signal restoration techniques, the experiment demonstrated how limited bandwidth can distort digital signals and how **signal restoration circuits** can recover the original digital waveform. This activity highlights important principles in **digital communication system design and signal integrity**.

---

### Introduction
In practical communication systems, signals are transmitted through channels that have **limited bandwidth**. These limitations can affect the quality of the transmitted signal, particularly in digital communication systems where sharp transitions between logic levels are required.

Bandwidth limitations can cause **distortion, rounding of digital pulses, and timing errors**, which may lead to incorrect decoding of digital information. Understanding how bandwidth affects signal transmission and learning methods to restore distorted signals are essential skills in telecommunications and digital electronics.

---

### Theoretical Background
Digital signals ideally consist of **square waveforms with sharp transitions** between logic high and logic low levels. However, when these signals pass through channels with limited bandwidth, the high-frequency components required to produce sharp edges are removed.

As a result, the signal edges become **rounded and distorted**, which can affect timing and decoding accuracy.

Signal restoration circuits are used to correct these distortions. These circuits typically involve **comparators or digital reshaping circuits** that regenerate the signal by restoring the logic levels and transitions.

In PCM systems, proper signal restoration ensures that the **digital data stream can still be correctly decoded even after passing through a bandwidth-limited channel**.

---

# Discussion

---

### Part A – The Effects of Bandwidth Limiting on PCM Decoding
In this part of the experiment, the PCM signal was passed through a **bandwidth-limited channel** before reaching the decoder. The limited bandwidth removed some of the higher frequency components of the signal, causing distortion in the digital waveform.

Despite this distortion, the PCM decoder was still able to interpret the digital data under certain conditions.

- **Purpose:** Observe how bandwidth limitation affects PCM decoding  
- **Observation:** Digital pulses became slightly distorted after passing through the limited bandwidth channel  
- **Result:** The PCM signal could still be decoded, but excessive bandwidth limitation may lead to decoding errors


---

### Part B – Effects of Bandwidth Limiting on a Digital Signal's Shape
In this section, the waveform of the digital signal was examined after passing through a bandwidth-limited channel. Ideally, digital signals should have **sharp rising and falling edges**, but bandwidth limitation removed the higher-frequency harmonics needed to maintain this shape.

As a result, the digital waveform appeared **rounded and smoother**, with slower transitions between logic levels.

- **Purpose:** Observe waveform distortion due to bandwidth limitations  
- **Observation:** Square wave signals become rounded and less defined  
- **Result:** The digital signal loses its ideal shape due to the removal of high-frequency components

<details>
<summary>View Part B Image Result</summary>

<p align="center">
<img src="Results/laboratory files 14/14BPART1.png" alt="Digital Signal Shape After Bandwidth Limiting" width="600">
</p>

</details>

---

### Part C – Restoring Digital Signals
To correct the distortion caused by bandwidth limitation, a **signal restoration circuit** was used. This circuit reshapes the distorted waveform and restores it to a **clean digital signal** with clear logic levels.

Typically, a comparator or digital reshaping circuit is used to regenerate the waveform by forcing the signal to switch between fixed voltage levels.

- **Purpose:** Recover the original digital signal after distortion  
- **Observation:** The restored waveform regains sharper transitions and clear logic levels  
- **Result:** The digital signal was successfully regenerated and became suitable for reliable decoding

<details>
<summary>View Part C Image Result</summary>

<p align="center">
<img src="Results/laboratory files 14/14BPART2.png" alt="Restored Digital Signal" width="600">
</p>

</details>

---

### Key Takeaways
- Real communication channels have **limited bandwidth**, which affects signal quality.
- Bandwidth limitation removes **high-frequency components** needed for sharp digital transitions.
- Digital signals become **rounded and distorted** when transmitted through a bandwidth-limited channel.
- **Signal restoration circuits** regenerate distorted digital signals for accurate decoding.
