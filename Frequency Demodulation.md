# EMONA Frequency Demodulation Experiment

---

### Abstract
This experiment focused on the **demodulation of Frequency Modulated (FM) signals** using the EMONA telecommunications trainer. The objective was to study the process of recovering the original message signal from an FM waveform using a **Zero-Crossing Detector (ZCD)**. Through several stages, including the setup of the FM modulator and ZCD circuit, the experiment demonstrated how frequency variations in the carrier can be converted into amplitude variations corresponding to the original message. The experiment reinforces key concepts such as **frequency deviation, signal conversion, and waveform detection**, which are fundamental in communication systems.

---

### Introduction
Frequency Modulation (FM) is widely used in communication systems because of its **high immunity to noise and interference**. However, for information to be useful, the modulated signal must be **demodulated**, meaning the original message must be recovered from the modulated carrier.

One technique used for FM demodulation is the **Zero-Crossing Detector (ZCD)**. This method converts frequency variations of the FM signal into **pulse-width variations**, which can then be filtered to recover the original message signal. Understanding this process helps students visualize how **frequency variations can be transformed back into amplitude-based information**.

---

### Theoretical Background
In an FM signal, the **instantaneous frequency of the carrier varies according to the amplitude of the message signal**. To recover the message, the demodulation circuit must convert these frequency changes into a measurable signal.

A **comparator-based zero-crossing detector** works by detecting when the input signal crosses zero volts. Each time the signal crosses zero, the comparator switches state, producing a **square wave output**. The frequency of this square wave corresponds to the frequency of the FM signal.

By passing this output through a **pulse shaping and filtering process**, the varying pulse widths represent the frequency variations of the FM signal, which can then be converted back into the original message waveform.

---

# Discussion

---

### Part A – Setting Up the FM Modulator
In this part, the FM modulator was configured to generate a **frequency-modulated carrier signal**. A message signal was applied to vary the frequency of the carrier according to the principles of FM. This setup forms the basis for the demodulation experiment since the generated FM signal will later be processed by the zero-crossing detector.

- **Purpose:** Generate an FM signal for demodulation experiments  
- **Observation:** Carrier frequency varies according to the input message  
- **Result:** A properly modulated FM waveform was produced

<details>
<summary>View Part A Image Result</summary>
<p align="center"> <img src="Results/laboratory report 10/10-Part-A-1-FM.png"alt="FM Modulator Setup" width="600"> </p>
<p align="center"> <img src="Results/laboratory report 11/11.2.jpg" alt="Zero Crossing Detector Setup" width="600"> </p>
</details>

---

### Part B – Setting Up the Zero-Crossing Detector
The Zero-Crossing Detector (ZCD) was configured using a **comparator circuit** to detect the zero crossings of the FM signal. Each time the FM waveform crosses zero volts, the comparator switches between high and low states, producing a **square wave output**.

- **Purpose:** Convert the FM waveform into a digital-like signal  
- **Observation:** Output waveform changes state at each zero crossing  
- **Result:** The output frequency matches the instantaneous frequency of the FM signal

<details>
<summary>View Part B Image Result</summary>
<p align="center"> <img src="Results/laboratory report 11/11.4.jpg" alt="Zero Crossing Detector Setup" width="600"> </p>

</details>

---

### Part C – Investigating the Operation of the Zero-Crossing Detector

**Why is the FM signal no longer a sine wave?**  
After passing through the comparator, the analog sine wave is converted into a **digital-like waveform** because the comparator only outputs two voltage levels (high or low).

**What type of waveform does the comparator output?**  
The comparator produces a **square wave** corresponding to the zero crossings of the FM signal.

**What does this tell us about the DC component of the comparator's output?**  
The square wave contains a **DC component determined by the duty cycle** of the waveform.

After passing through the **twin pulse generator and comparator**, the output waveform becomes a **series of pulses**.

**What type of waveform does the ZCD output?**  
The ZCD outputs a **pulse train** where the spacing between pulses depends on the frequency of the FM signal.

**As the FM signal changes frequency, so does the ZCD's output. What aspect of the signal changes?**  
The **pulse spacing (or pulse repetition rate)** changes. Higher frequency produces **closer pulses**, while lower frequency produces **wider spacing**.

**What does this tell us about the DC component of the comparator output?**  
The **average DC level varies depending on the pulse density**, which reflects the frequency variation of the original FM signal.

<details>
<summary>View Part C Image Result</summary>
<p align="center"> <img src="Results/laboratory report 11/11.5.jpg" alt="Zero Crossing Detector Output" width="600"> </p>

<p align="center"> <img src="Results/laboratory report 11/11.6.jpg" alt="Zero Crossing Detector Output" width="600"> </p>

<p align="center"> <img src="Results/laboratory report 11/11.7.jpg" alt="Zero Crossing Detector Output" width="600"> </p>

</details>

---

### Part D – Transmitting and Recovering a Sine Wave Using FM
In this part, a **sine wave message signal** was transmitted using FM and then demodulated using the ZCD circuit. After filtering the pulse output, the recovered signal resembled the original sine wave message.

- **Observation:** The recovered waveform closely matches the original sine wave  
- **Purpose:** Demonstrate successful FM demodulation using a ZCD method

<details>
<summary>View Part D Image Result</summary>
<p align="center"> <img src="Results/laboratory report 11/11.8.jpg" alt="Recovered Sinewave from FM" width="600"> </p>

</details>

---

### Part E – Transmitting and Recovering Speech Using FM
Finally, a **speech signal** was transmitted using FM modulation and recovered through the demodulation circuit. The recovered audio demonstrated that the ZCD technique can successfully retrieve complex message signals such as speech.

- **Observation:** Recovered speech signal retains the characteristics of the original message  
- **Purpose:** Demonstrate practical FM communication and demodulation

<details>
<summary>View Part E Image Result</summary>
<p align="center"> <img src="Results/laboratory report 11/11.5.jpg" alt="Recovered Speech from FM" width="600"> </p>
</details>
