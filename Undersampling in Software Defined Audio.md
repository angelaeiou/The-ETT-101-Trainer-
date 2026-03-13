# Undersampling in Software Defined Audio

---

### Abstract
This experiment explored the concept of **undersampling (bandpass sampling)** in software-defined audio systems. The objective was to demonstrate how a **bandwidth-limited signal** can be directly down-converted by sampling it at a rate lower than the Nyquist frequency, without using a traditional mixer. The experiment also examined the importance of **synchronization** in maintaining proper signal reconstruction. The results show how undersampling can effectively translate high-frequency signals into lower frequencies when properly configured.

---

### Introduction
In traditional signal processing systems, down-conversion is performed using a mixer and local oscillator. However, in **software-defined systems**, frequency translation can also be achieved through **undersampling**.

Undersampling occurs when a signal is sampled at a rate that is intentionally lower than twice its highest frequency component. When the signal is **bandwidth-limited**, this technique can shift the signal spectrum to a lower frequency range, effectively performing **direct down-conversion**.

This method is widely used in **software-defined radio (SDR)** and digital communication systems.

---

### Theoretical Background

According to the **Nyquist Theorem**, a signal must be sampled at a rate:

\[
f_s \geq 2f_{max}
\]

to avoid aliasing.

However, if the signal is **bandpass-limited** (meaning it occupies a specific frequency band rather than starting at 0 Hz), it is possible to use a lower sampling rate. In this case:

- The sampled spectrum folds into lower frequencies.
- The desired signal band shifts to baseband.
- Proper filtering is required to avoid overlapping spectral components.

This process is known as **bandpass sampling or undersampling**.

---

# Discussion

---

### Part A – Setting Up a Bandwidth-Limited Signal

In this part, the signal was first configured to ensure it was **bandwidth-limited**. This is important because undersampling only works correctly when the signal occupies a controlled frequency band.

A filtering stage was used to restrict the signal’s bandwidth. This prevents unwanted spectral overlap after sampling.

- **Purpose:** Prepare the signal for undersampling  
- **Observation:** Signal bandwidth was limited before sampling  
- **Result:** Signal is suitable for direct down-conversion  

<details>
<summary>View Part A Image Result</summary>

<p align="center">
<img src="Results/laboratory results 20/E20APART1.png" alt="Bandwidth Limited Signal Setup" width="600">
</p>

</details>

---

### Part B – Direct Down-Conversion Using Undersampling

In this section, the bandwidth-limited signal was sampled at a rate lower than the Nyquist rate.

Due to undersampling:

- The signal spectrum was shifted to a lower frequency.
- No traditional mixer was required.
- Frequency translation occurred through aliasing.

This demonstrates how undersampling can act as a **direct down-conversion technique** in software-defined systems.

- **Purpose:** Achieve frequency translation using sampling  
- **Observation:** Signal shifted to lower frequency range  
- **Result:** Successful down-conversion through undersampling  

<details>
<summary>View Part B Image Result</summary>

<p align="center">
<img src="Results/laboratory results 20/E20PARTBPART1.png" alt="Direct Down Conversion Using Undersampling" width="600">
<img src="Results/laboratory results 20/E20BPART2.png" alt="Direct Down Conversion Using Undersampling" width="600">
</p>

</details>

---

### Part C – Synchronization

Synchronization is critical in undersampling systems.

For proper signal reconstruction:

- The sampling clock must be stable.
- The sampling frequency must be accurately controlled.
- Any timing mismatch may distort the recovered signal.

Without proper synchronization, aliasing may cause signal distortion or incorrect frequency placement.

This part demonstrates that successful undersampling depends heavily on **clock and frequency synchronization**.

- **Purpose:** Ensure correct signal reconstruction  
- **Observation:** Stable sampling clock improves output accuracy  
- **Result:** Proper synchronization enables reliable down-conversion  

<details>
<summary>View Part C Image Result</summary>

<p align="center">
<img src="Results/laboratory results 20/E20CPART1.png" alt="Synchronization in Undersampling" width="600">
</p>

</details>

---

### Key Takeaways

- Undersampling can perform **direct down-conversion** without a mixer.
- It works only for **bandwidth-limited (bandpass) signals**.
- The technique relies on controlled aliasing.
- Proper **synchronization** is essential for accurate reconstruction.
- This method is widely used in **software-defined audio and SDR systems**.
