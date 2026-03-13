# Quadrature Phase Shift Keying (QPSK) Experiment

---

### Abstract
This experiment investigated the operation of **Quadrature Phase Shift Keying (QPSK)** modulation using the EMONA telecommunications trainer. The objective was to observe how digital information can be transmitted by shifting the phase of a carrier signal among four distinct states. The experiment involved generating a QPSK signal and using **phase discrimination techniques** to separate the QPSK waveform into its underlying **Binary Phase Shift Keying (BPSK) components**. This activity demonstrates how QPSK efficiently transmits digital data by encoding two bits per symbol.

---

### Introduction
Quadrature Phase Shift Keying (QPSK) is an advanced digital modulation technique that extends the concept of **Binary Phase Shift Keying (BPSK)**. Instead of using only two phase states, QPSK uses **four phase states**, typically separated by 90°. This allows the system to transmit **two bits of information per symbol**, effectively doubling the data rate compared to BPSK for the same bandwidth.

QPSK is widely used in **satellite communication, wireless networks, and modern digital broadcasting systems**. At the receiver, phase discrimination techniques are used to determine which phase state was transmitted, allowing the original digital data streams to be recovered.

---

### Theoretical Background
In a QPSK system, the input digital data stream is divided into two parallel streams:

- **In-phase component (I)**
- **Quadrature component (Q)**

Each component modulates a carrier signal. The Q component is shifted by **90°** relative to the I component. When these two modulated signals are combined, the resulting waveform has **four possible phase states**:

- 0°
- 90°
- 180°
- 270°

Each phase state represents a **unique pair of binary bits**. At the receiver, phase discrimination or coherent detection techniques are used to separate the QPSK signal back into its **two BPSK components**, allowing the original digital information to be recovered.

---

# Discussion

---

### Part A – Generating a QPSK Signal
In this part of the experiment, the QPSK modulator was configured to generate a carrier signal whose phase changes among **four possible states** depending on the digital input data.

Two digital data streams were applied to the modulator, representing the **in-phase (I) and quadrature (Q) components**. These signals modulated two carriers that were **90° out of phase**, producing the final QPSK waveform.

- **Purpose:** Generate a digital signal using quadrature phase modulation  
- **Observation:** The carrier signal shifts among four distinct phase positions  
- **Result:** A QPSK waveform representing pairs of digital bits was successfully generated

<details>
<summary>View Part A Image Result</summary>

<p align="center">
<img src="QPSK/IMG_PartA.png" alt="Generated QPSK Signal" width="600">
</p>

</details>

---

### Part B – Using Phase Discrimination to Pick Out the QPSK Signal's BPSK Components
In this section, **phase discrimination techniques** were used to separate the QPSK signal into its two underlying **BPSK signals**.

The received QPSK signal was processed using detection circuits that compared the signal with reference carriers. This allowed the receiver to determine the **in-phase (I) and quadrature (Q) components**, effectively extracting the two BPSK signals embedded within the QPSK waveform.

- **Purpose:** Separate the QPSK signal into its component BPSK signals  
- **Observation:** Two independent digital signals corresponding to the I and Q components were obtained  
- **Result:** The original digital data streams were successfully identified through phase discrimination

<details>
<summary>View Part B Image Result</summary>

<p align="center">
<img src="QPSK/IMG_PartB.png" alt="Phase Discrimination of QPSK Signal" width="600">
</p>

</details>

---

### Key Takeaways
- QPSK transmits **two bits per symbol** by using four carrier phase states.
- The modulation process combines **two BPSK signals (I and Q components)**.
- The carriers used in QPSK are **90° out of phase** with each other.
- **Phase discrimination techniques** allow the receiver to separate the QPSK signal into its component BPSK signals and recover the original digital data.
