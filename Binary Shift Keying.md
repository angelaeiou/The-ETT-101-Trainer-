# Binary Phase Shift Keying (BPSK) Experiment

---

### Abstract
This experiment explored the principles of **Binary Phase Shift Keying (BPSK)** modulation and demodulation using the EMONA telecommunications trainer. The objective was to observe how digital information can be transmitted by altering the **phase of a carrier signal**. The experiment involved generating a BPSK signal, demodulating it using a **product detector**, and restoring the digital signal using a **comparator circuit**. This activity demonstrates the fundamental concepts behind **phase modulation techniques widely used in digital communication systems**.

---

### Introduction
Binary Phase Shift Keying (BPSK) is a form of **digital phase modulation** where the phase of a carrier signal is changed according to the binary input data. Unlike amplitude or frequency modulation, BPSK represents digital information by shifting the phase of the carrier between two states, typically **0° and 180°**.

This technique is widely used in **satellite communication, wireless networks, and digital radio systems** because it offers strong resistance to noise and interference. To recover the original digital data, the receiver must detect the phase changes of the carrier signal using a **coherent detection method**, such as a product detector.

---

### Theoretical Background
In a **BPSK system**, a sinusoidal carrier signal is multiplied by the digital message signal. When the input data is **logic 1**, the carrier is transmitted without phase change. When the input data is **logic 0**, the carrier undergoes a **180° phase shift**.

The resulting waveform maintains a constant amplitude but changes phase according to the digital data pattern.

To demodulate the signal, a **product detector** multiplies the received signal with a locally generated reference carrier that is synchronized with the transmitter. This process converts the phase variations into amplitude variations corresponding to the original digital signal.

Finally, a **comparator circuit** restores the recovered waveform into a clean digital signal by applying a threshold that separates logic high and logic low levels.

---

# Discussion

---

### Part A – Generating a BPSK Signal
In this part of the experiment, the BPSK modulator was configured to produce a carrier signal whose **phase changes according to the digital input data**. When the digital input changed between logic states, the carrier waveform experienced a **phase reversal of 180°**.

- **Purpose:** Generate a phase-modulated carrier representing digital data  
- **Observation:** The carrier waveform flips phase whenever the input data changes  
- **Result:** A BPSK waveform representing the digital message signal was successfully generated

<details>
<summary>View Part A Image Result</summary>

<p align="center">
<img src="Results/laboratory files 17/PART-A-fig2.png" alt="Generated BPSK Signal" width="600">
</p>

</details>

---

### Part B – Demodulating a BPSK Signal Using a Product Detector
In this section, the received BPSK signal was passed through a **product detector**, which multiplies the signal with a reference carrier signal. This process converts the phase variations into amplitude variations that correspond to the original digital data.

The resulting output waveform shows positive and negative voltage levels depending on the phase of the received signal.

- **Purpose:** Recover the message signal from the BPSK waveform  
- **Observation:** The output waveform reflects the phase changes of the received signal  
- **Result:** The digital data pattern was successfully extracted from the BPSK signal

<details>
<summary>View Part B Image Result</summary>

<p align="center">
<img src="Results/laboratory files 17/PART-B-fig4.png" alt="BPSK Demodulation Using Product Detector" width="600">
</p>

</details>

---

### Part C – Restoring the Recovered Digital Signal Using a Comparator
After demodulation, the recovered signal may contain noise or slight distortions. A **comparator circuit** was used to restore the waveform into a clean digital signal by comparing the signal amplitude to a reference threshold.

The comparator forces the output to switch between defined logic levels, producing a clear digital waveform.

- **Purpose:** Regenerate the digital signal after demodulation  
- **Observation:** Output waveform becomes a stable square wave  
- **Result:** The original digital message signal was successfully restored

<details>
<summary>View Part C Image Result</summary>

<p align="center">
<img src="Results/laboratory files 17/PART-C-fig6.png" alt="Restored Digital Signal After BPSK Demodulation" width="600">
</p>

</details>

---

### Key Takeaways
- BPSK transmits digital information by **changing the phase of the carrier signal**.
- The two phase states typically represent **binary 0 and binary 1**.
- A **product detector** converts phase changes into amplitude variations for demodulation.
- A **comparator circuit restores the recovered signal** into a clean digital waveform.
