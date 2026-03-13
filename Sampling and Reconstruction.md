# Sampling and Reconstruction Experiment

---

### Abstract
This experiment focused on the process of **sampling analog signals and reconstructing them back into continuous waveforms** using the EMONA telecommunications trainer. The objective was to understand how analog signals can be converted into discrete-time signals and later reconstructed without losing information. Through the sampling of a simple waveform and speech signals, as well as the investigation of aliasing, the experiment demonstrated the importance of the **sampling theorem and reconstruction filtering** in digital communication systems.

---

### Introduction
Modern communication and signal processing systems rely heavily on the **conversion of analog signals into digital form**. This process involves sampling, where the continuous signal is measured at regular time intervals. Once sampled, the signal can be stored, transmitted, or processed digitally.

However, for the signal to be accurately recovered, the **sampling frequency must be sufficiently high**. If the sampling rate is too low, distortion known as **aliasing** occurs. Understanding these principles is essential in telecommunications, digital audio processing, and data acquisition systems.

---

### Theoretical Background
Sampling is the process of converting a **continuous-time signal into a discrete-time signal** by measuring the amplitude of the signal at periodic intervals. According to the **Nyquist Sampling Theorem**, the sampling frequency must be at least **twice the highest frequency component of the message signal** to allow perfect reconstruction.

After sampling, the signal becomes a **pulse amplitude modulated (PAM) waveform**, where the amplitude of each pulse represents the instantaneous value of the original signal. To recover the original signal, the sampled waveform is passed through a **reconstruction filter**, which removes high-frequency components introduced during the sampling process.

Aliasing occurs when the sampling frequency is **lower than twice the message frequency**, causing different frequency components to become indistinguishable. This results in distortion where the reconstructed signal appears at a lower frequency than the original.

---

# Discussion

---

### Part A – Sampling a Simple Message
In this part, a **simple message signal**, typically a sine wave, was applied to the sampling circuit. The sampling module generated pulses at a fixed sampling frequency, producing a **pulse amplitude modulated (PAM) signal**.

Each pulse represented the instantaneous amplitude of the input signal at the sampling moment.

- **Purpose:** Observe how an analog signal becomes a discrete-time signal  
- **Observation:** Output waveform consists of pulses following the amplitude of the input signal  
- **Result:** A sampled waveform representing the original sine wave was produced

<details>
<summary>View Part A Image Result</summary>
<p align="center"> <img src="Sampling/IMG_PartA.png" alt="Sampling Simple Message" width="600"> </p>
</details>

---

### Part B – Sampling Speech
In this section, a **speech signal** was used as the message input. Speech contains multiple frequency components and varying amplitudes, making it a more complex signal compared to a simple sine wave.

When sampled, the speech waveform produced a **PAM signal whose pulse amplitudes varied rapidly**, reflecting the characteristics of the spoken message.

- **Purpose:** Demonstrate sampling of real-world signals  
- **Observation:** Sampled waveform shows irregular pulse amplitudes corresponding to speech variations  
- **Result:** Speech signal successfully converted into a sampled representation

<details>
<summary>View Part B Image Result</summary>
<p align="center"> <img src="Sampling/IMG_PartB.png" alt="Sampling Speech Signal" width="600"> </p>
</details>

---

### Part C – Reconstructing a Sampled Message
After sampling, the PAM signal was passed through a **reconstruction filter** to recover the original continuous waveform. The filter removes the high-frequency components introduced by the sampling process and smooths the waveform.

The output signal closely resembled the original message signal when the **sampling frequency satisfied the Nyquist criterion**.

- **Purpose:** Recover the original analog signal from sampled pulses  
- **Observation:** Filtered waveform becomes smooth and similar to the original signal  
- **Result:** Successful reconstruction of the input message signal

<details>
<summary>View Part C Image Result</summary>
<p align="center"> <img src="Sampling/IMG_PartC.png" alt="Reconstructed Signal" width="600"> </p>
</details>

---

### Part D – Aliasing
In this part, the sampling frequency was intentionally **reduced below the Nyquist rate** to observe the effects of aliasing. When the sampling frequency becomes too low, the reconstructed signal no longer represents the original waveform correctly.

Instead, the output appears as a **lower-frequency waveform**, which is not present in the original signal.

- **Purpose:** Demonstrate the effects of undersampling  
- **Observation:** Reconstructed signal frequency differs from the original  
- **Result:** Aliasing distortion occurs when the sampling frequency is insufficient

<details>
<summary>View Part D Image Result</summary>
<p align="center"> <img src="Sampling/IMG_PartD.png" alt="Aliasing Observation" width="600"> </p>
</details>

---

### Key Takeaways
- Sampling converts **continuous-time signals into discrete-time signals**.
- The **Nyquist Sampling Theorem** states that the sampling frequency must be at least **twice the highest signal frequency**.
- Reconstruction filters are used to **recover the original waveform** from sampled signals.
- **Aliasing occurs when the sampling frequency is too low**, causing distortion in the reconstructed signal.
