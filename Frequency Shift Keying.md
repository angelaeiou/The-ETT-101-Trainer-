# Frequency Shift Keying (FSK) Experiment

---

### Abstract
This experiment explored the principles of **Frequency Shift Keying (FSK)** modulation and demodulation using the EMONA telecommunications trainer. The objective was to observe how digital information can be transmitted by switching between two different carrier frequencies. The experiment involved generating an FSK signal, recovering the message using filtering and an envelope detector, and restoring the digital signal using a comparator. This activity demonstrates the operation of **digital frequency modulation techniques commonly used in communication systems**.

---

### Introduction
Frequency Shift Keying (FSK) is a type of **digital modulation technique** in which the frequency of a carrier signal is varied according to the binary input data. Instead of changing amplitude or phase, FSK transmits digital information by switching between two distinct frequencies.

This method is widely used in **wireless communication systems, data transmission, and telemetry applications** because of its robustness against noise and signal interference.

To recover the original digital data, the receiver separates the two frequencies using **filters** and then detects the signal using an **envelope detector**, followed by a **comparator** to restore the digital waveform.

---

### Theoretical Background
In a basic **Binary Frequency Shift Keying (BFSK)** system, two carrier frequencies represent the binary states:

- **Mark Frequency (f₁):** Represents binary 1  
- **Space Frequency (f₂):** Represents binary 0  

When the input data changes between logic levels, the transmitted carrier switches between these two frequencies. The resulting waveform is called the **FSK signal**.

At the receiver, **band-pass filters** are used to separate the two frequencies. The output signals are then passed through **envelope detectors**, which convert the frequency variations into amplitude variations corresponding to the original digital data. Finally, a **comparator circuit** restores the signal into a clean digital waveform.

---

# Discussion

---

### Part A – Generating an FSK Signal
In this part of the experiment, the FSK modulator was configured to generate a waveform in which the carrier frequency switched between two values depending on the input digital signal.

When the digital input was **logic high**, the modulator produced one carrier frequency, and when the input was **logic low**, the modulator generated a different frequency.

- **Purpose:** Generate a digital signal using frequency shift keying  
- **Observation:** Output waveform alternates between two distinct frequencies  
- **Result:** An FSK signal representing the digital message was successfully generated

<details>
<summary>View Part A Image Result</summary>

<p align="center">
<img src="Results/laboratory files 16/E16A.png" alt="Generated FSK Signal" width="600">
<img src="Results/laboratory files 16/E16APART2.png" alt="Generated FSK Signal" width="600">
</p>

</details>

---

### Part B – Demodulating an FSK Signal Using Filtering and an Envelope Detector
In this section, the received FSK signal was passed through **frequency-selective filters** to separate the two carrier frequencies. Each filtered signal was then processed by an **envelope detector**, which converted the frequency variations into amplitude changes.

These amplitude variations corresponded to the original digital data pattern.

- **Purpose:** Recover the message signal from the FSK waveform  
- **Observation:** Filter outputs correspond to the presence of specific carrier frequencies  
- **Result:** The envelope detector produced a waveform resembling the original digital signal

<details>
<summary>View Part B Image Result</summary>

<p align="center">
<img src="Results/laboratory files 16/E16BPART1.png" alt="FSK Demodulation Using Filters and Envelope Detector" width="600">
<img src="Results/laboratory files 16/E16BPART2.png" alt="FSK Demodulation Using Filters and Envelope Detector" width="600">
</p>

</details>

---

### Part C – Restoring the Recovered Digital Signal Using a Comparator
After demodulation, the recovered signal may appear distorted or contain noise. To restore the signal into a clean digital waveform, a **comparator circuit** was used.

The comparator compares the signal to a reference threshold and produces a digital output with clear logic high and logic low levels.

- **Purpose:** Regenerate the digital signal after demodulation  
- **Observation:** Output waveform becomes a clean square digital signal  
- **Result:** The original digital data stream was successfully restored

<details>
<summary>View Part C Image Result</summary>

<p align="center">
<img src="Results/laboratory files 16/E16CPART1.png" alt="Restored Digital Signal After FSK Demodulation" width="600">
</p>

</details>

---

### Key Takeaways
- FSK transmits digital information by **switching between two carrier frequencies**.
- Frequency-selective **filters separate the two frequencies** at the receiver.
- **Envelope detectors** convert the separated signals into amplitude variations.
- A **comparator circuit restores the recovered signal** into a clean digital waveform.
