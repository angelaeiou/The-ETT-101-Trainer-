# PCM Encoding Experiment

---

### Abstract
This experiment explored the principles of **Pulse Code Modulation (PCM) encoding** using the EMONA telecommunications trainer. The objective was to observe how analog voltage signals are converted into digital binary codes through the processes of **sampling, quantization, and encoding**. By first applying a static DC voltage and later varying the input signal, the experiment demonstrated how PCM systems represent different voltage levels as digital values. The activity highlights the fundamental concepts behind **digital signal representation and digital communication systems**.

---

### Introduction
Pulse Code Modulation (PCM) is a method used to convert **analog signals into digital data**. It is widely used in modern communication systems such as **digital telephony, audio recording, and data transmission**. PCM works by periodically sampling an analog signal, assigning each sample to the nearest quantization level, and representing that level using a binary code.

Understanding PCM encoding is essential because most real-world signals such as **speech, audio, and sensor data** must be converted into digital form before they can be stored or transmitted in modern communication systems.

---

### Theoretical Background
PCM encoding involves three main stages:

1. **Sampling** – Measuring the amplitude of an analog signal at discrete time intervals.
2. **Quantization** – Approximating each sampled value to the nearest predefined amplitude level.
3. **Encoding** – Converting the quantized value into a binary number for digital transmission.

If the analog signal changes slowly, the PCM output changes gradually between binary values. However, if the signal changes continuously, the encoder constantly updates the binary output to represent the varying amplitude levels.

Quantization introduces a small error known as **quantization noise**, which occurs because the exact analog value may fall between two quantization levels.

---

# Discussion

---

### Part A – An Introduction to PCM Encoding Using a Static DC Voltage
In this part of the experiment, a **constant DC voltage** was applied to the PCM encoder input. Since the input voltage does not change with time, the encoder produces a **constant digital output code** corresponding to that voltage level.

This demonstrates how a PCM encoder converts a single analog value into a **specific binary representation**.

- **Purpose:** Observe how a fixed analog voltage is encoded into a digital value  
- **Observation:** The PCM output remains constant because the input voltage does not change  
- **Result:** A stable binary code representing the input voltage was generated

<details>
<summary>View Part A Image Result</summary>

<p align="center">
<img src="PCM/IMG_PCM_PartA.png" alt="PCM Static DC Voltage Encoding" width="600">
</p>

</details>

---

### Part B – PCM Encoding of a Variable DC Voltage
In this section, the DC voltage input was gradually adjusted. As the input voltage changed, the PCM encoder updated the **binary output code** to represent the new quantization level.

Each small change in input voltage caused the digital output to shift to the **next quantization level**.

- **Purpose:** Observe how changes in analog voltage affect the digital output  
- **Observation:** The PCM code changes whenever the input crosses a quantization boundary  
- **Result:** The encoder produced different binary codes corresponding to the varying voltage levels

<details>
<summary>View Part B Image Result</summary>

<p align="center">
<img src="PCM/IMG_PCM_PartB.png" alt="PCM Variable DC Voltage Encoding" width="600">
</p>

</details>

---

### Part C – Quantisation
Quantization is the process of mapping a continuous range of analog voltages into a **finite number of discrete levels**. In the PCM encoder, each sampled value is approximated to the **nearest quantization level**, which is then converted into a binary number.

Because the actual analog value may not exactly match a quantization level, a **quantization error** occurs. This difference between the original signal and the quantized value is known as **quantization noise**.

- **Purpose:** Understand how analog signals are approximated into discrete digital levels  
- **Observation:** Small changes in voltage may not immediately change the digital output until a new level is reached  
- **Result:** The PCM output steps between discrete binary values

<details>
<summary>View Part C Image Result</summary>

<p align="center">
<img src="PCM/IMG_PCM_PartC.png" alt="Quantisation Levels" width="600">
</p>

</details>

---

### Part D – PCM Encoding of Continuously Changing Voltages
In the final part, a continuously varying signal was applied to the PCM encoder. As the signal changed over time, the encoder repeatedly sampled the signal and produced a **sequence of binary codes** representing the instantaneous amplitude of the input signal.

This demonstrates how PCM can represent **dynamic signals such as audio or speech** in digital form.

- **Purpose:** Observe PCM encoding of continuously changing analog signals  
- **Observation:** Binary output constantly changes to follow the variations of the input signal  
- **Result:** A stream of digital codes representing the analog waveform was produced

<details>
<summary>View Part D Image Result</summary>

<p align="center">
<img src="PCM/IMG_PCM_PartD.png" alt="PCM Encoding Continuous Signal" width="600">
</p>

</details>

---

### Key Takeaways
- PCM converts **analog signals into digital binary codes**.
- The encoding process includes **sampling, quantization, and binary encoding**.
- **Quantization introduces small errors** because analog values are approximated to discrete levels.
- Continuously varying signals produce a **continuous stream of digital codes** representing the waveform.
