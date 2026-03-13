# Amplitude Shift Keying (ASK) Experiment

---

### Abstract
This experiment investigated the principles of **Amplitude Shift Keying (ASK)** modulation and demodulation using the EMONA telecommunications trainer. The objective was to observe how digital data can be transmitted by varying the amplitude of a carrier signal and how the original digital information can be recovered at the receiver. Through the generation of an ASK signal, demodulation using an envelope detector, and restoration using a comparator circuit, the experiment demonstrated the fundamental processes involved in **digital amplitude modulation systems**.

---

### Introduction
Amplitude Shift Keying (ASK) is a form of **digital modulation** where the amplitude of a carrier signal is varied according to the digital input data. In its simplest form, the carrier signal is present for a binary **logic 1** and absent (or reduced) for a **logic 0**.

ASK modulation is commonly used in **low-cost digital communication systems**, radio frequency identification (RFID), and optical communication. To recover the transmitted data, the receiver must detect the envelope of the modulated signal and convert it back into digital form.

Understanding ASK modulation and demodulation is important for studying **digital communication techniques and signal detection methods**.

---

### Theoretical Background
In ASK modulation, the amplitude of a sinusoidal carrier is controlled by a digital message signal. When the message signal is high (logic 1), the carrier is transmitted at full amplitude. When the message signal is low (logic 0), the carrier amplitude is reduced or removed.

The demodulation process involves detecting the **envelope of the ASK waveform**. An envelope detector extracts the amplitude variations of the signal, producing a waveform that follows the original digital data pattern.

However, the recovered signal may contain noise or distortion. Therefore, a **comparator circuit** is often used to restore the waveform into a clean digital signal by forcing it into clear logic high and logic low levels.

---

# Discussion

---

### Part A – Getting an ASK Signal
In this part of the experiment, the ASK modulator was configured to generate a modulated carrier signal using a digital input message. The carrier signal's amplitude varied depending on the state of the input digital signal.

When the digital input was high, the carrier signal appeared at the output. When the digital input was low, the carrier amplitude was significantly reduced or absent.

- **Purpose:** Generate an ASK modulated signal  
- **Observation:** Carrier signal appears only during logic high periods of the message signal  
- **Result:** A waveform showing amplitude variations corresponding to the digital data was observed

<details>
<summary>View Part A Image Result</summary>

<p align="center">
<img src="ASK/IMG_PartA.png" alt="ASK Modulated Signal" width="600">
</p>

</details>

---

### Part B – Demodulating an ASK Signal Using an Envelope Detector
In this section, the ASK signal was passed through an **envelope detector** to extract the amplitude variations of the signal. The envelope detector removes the carrier component and produces a waveform that follows the shape of the digital message signal.

Although the output resembles the original digital signal, it may appear slightly distorted or rounded due to filtering effects.

- **Purpose:** Recover the message signal from the ASK waveform  
- **Observation:** Output waveform follows the envelope of the ASK signal  
- **Result:** The original digital data pattern was successfully extracted from the modulated signal

<details>
<summary>View Part B Image Result</summary>

<p align="center">
<img src="ASK/IMG_PartB.png" alt="Envelope Detector Output" width="600">
</p>

</details>

---

### Part C – Restoring the Recovered Digital Signal Using a Comparator
After envelope detection, the recovered signal was passed through a **comparator circuit** to restore the digital waveform. The comparator compares the signal to a reference threshold and produces a clean digital output with defined logic levels.

This process eliminates distortions and noise present in the envelope detector output.

- **Purpose:** Restore the recovered signal into a clean digital waveform  
- **Observation:** Output waveform shows clear logic high and logic low levels  
- **Result:** The original digital message signal was successfully reconstructed

<details>
<summary>View Part C Image Result</summary>

<p align="center">
<img src="ASK/IMG_PartC.png" alt="Restored Digital Signal" width="600">
</p>

</details>

---

### Key Takeaways
- ASK transmits digital data by **varying the amplitude of a carrier signal**.
- An **envelope detector** can recover the message signal from the modulated waveform.
- The recovered signal may contain distortions and requires **signal restoration**.
- A **comparator circuit** regenerates the digital signal by restoring clear logic levels.
