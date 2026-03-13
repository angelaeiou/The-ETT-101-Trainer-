# EMONA Frequency Modulation Experiment

---

### Abstract
This experiment focused on **Frequency Modulation (FM)** using both square wave and speech signals as message inputs. The objective was to familiarize students with **FM principles, signal generation, and spectral characteristics**, while observing the effect of **message amplitude and frequency on carrier deviation**. The experiment reinforces fundamental concepts such as **frequency deviation, modulation index, and sideband formation**, which are critical in communication engineering.

---

### Introduction
Frequency Modulation (FM) is a widely used modulation technique in **communications engineering**, where the **frequency of a carrier signal varies according to the amplitude of the input message signal**. FM is commonly used in **radio broadcasting, audio transmission, and communication systems**, as it provides **resistance to amplitude noise and interference**. 

Proper FM signal generation allows students to understand how **message signal characteristics (amplitude and frequency)** influence the carrier and its spectral composition.

---

### Theoretical Background
- **Frequency Modulation (FM):** The instantaneous frequency of the carrier is varied according to the amplitude of the message signal.  
- **Frequency Deviation (Δf):** The maximum shift of the carrier frequency from its unmodulated value.  
- **Modulation Index (β):** Ratio of frequency deviation to message frequency: \( \beta = \frac{\Delta f}{f_m} \)  
- **Spectral Composition:** FM produces **sidebands spaced at integer multiples of the message frequency**, with amplitudes determined by **Bessel functions**.  
- **Message Signals:**  
  - Square wave → produces discrete frequency steps  
  - Speech signal → produces smooth, continuous carrier frequency variations  

---

### Discussion

#### Part A – Frequency Modulation of a Square Wave
In this part, a **square wave signal** was used as the message. The square wave causes the **carrier frequency to switch between discrete values**, demonstrating **FM principles** with a simple digital-like input.  

- **Message Signal:** Square wave  
- **Carrier:** Continuous RF signal  
- **Observation:** Discrete frequency jumps in the modulated carrier  
- **Purpose:** Demonstrate FM with a digital-like message signal  

<details>
<summary>View Part A Image Result</summary>
<p align="center"> <img src="Results/lab report files 9/9.1.jpg" alt="FM Square Wave Output" width="600"> </p>
</details>

---

#### Part B – Generating FM Signal Using a Speech Signal
This part uses a **speech waveform as the message** to generate a continuous FM signal. Smooth amplitude variations in the speech cause **continuous carrier frequency deviations**, simulating real-world FM signals.  

- **Message Signal:** Speech  
- **Carrier:** High-frequency RF  
- **Observation:** Continuous frequency deviation corresponding to message amplitude  
- **Purpose:** Observe practical FM modulation  

**Conceptual Questions – Part B**  
- **Relationship between FM signal frequency deviation and amplitude of the message:**  
  **Directly proportional.** Higher message amplitude → larger frequency deviation.  

- **Relationship between FM signal frequency deviation and frequency of the message:**  
  **Inversely affects the modulation index.** Higher message frequency → faster carrier frequency oscillations. Lower message frequency → slower changes.  

<details>
<summary>View Part B Image Result</summary>
<p align="center"> <img src="Results/lab report files 9/9.9.jpg" alt="FM Speech Output" width="600"> </p>
</details>

---

#### Part C – Considering the Spectral Composition of FM Signals
FM signals generate **sidebands spaced at integer multiples of the message frequency**. The number and amplitude of these sidebands depend on the **modulation index**, a function of both **message amplitude and frequency**. Compared to AM, FM signals have **wider bandwidths**, which can be estimated using **Carson’s rule**. Observing the spectral composition demonstrates **signal bandwidth and sideband structure**, important for communication system design.  

- **Observation:** Multiple sidebands appear around the carrier  
- **Purpose:** Analyze FM spectral composition and bandwidth  
- **Application:** FM broadcasting and communication systems  

<details>
<summary>View Part C Image Result</summary>
<p align="center"> <img src="Results/lab report files 9/9.11.jpg" alt="FM Spectral Output" width="600"> </p>
</details>

* [Other results from the experiment](https://github.com/angelaeiou/The-ETT-101-Trainer-/tree/main/Results/lab%20report%20files%209)
