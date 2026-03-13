# Direct Sequence Spread Spectrum (DSSS) Modulation and Demodulation

---

### Abstract
This experiment explored the principles of **Direct Sequence Spread Spectrum (DSSS)** modulation and demodulation using the EMONA telecommunications trainer. The objective was to observe how a message signal can be spread over a wider bandwidth using a **pseudo-random noise (PN) code**, and how the original message can be recovered using a **product detector**. The experiment also demonstrated the effect of **deliberate interference (jamming)** and how DSSS systems provide improved resistance to noise and interference.

---

### Introduction
Direct Sequence Spread Spectrum (DSSS) is a digital communication technique in which the original message signal is multiplied by a **high-rate spreading code**. This process spreads the signal energy over a much wider bandwidth than the original message bandwidth.

DSSS is widely used in **Wi-Fi, GPS, and secure military communication systems** because of its ability to resist interference and provide improved signal security. At the receiver, the same spreading code is used to **despread the signal**, allowing the original message to be recovered.

---

### Theoretical Background
In DSSS systems:

- The **message signal** is multiplied by a **pseudo-random noise (PN) code**.
- The PN code operates at a much higher frequency than the message signal.
- This multiplication spreads the signal across a wider frequency spectrum.
- The resulting signal appears noise-like.

At the receiver, a **product detector** multiplies the received signal with the same PN code. This process:

- Recovers the original message signal
- Spreads any interference across the bandwidth
- Reduces the effect of narrowband noise

This technique improves **noise immunity and signal robustness**.

---

# Discussion

---

### Part A – Generating a DSSS Signal Using a Simple Message
In this part, a **simple message signal** (such as a sine wave or digital waveform) was multiplied by a **spreading code** to generate the DSSS signal.

The output waveform appeared noise-like because the signal energy was spread over a wider bandwidth.

- **Purpose:** Generate a spread-spectrum signal using a basic message  
- **Observation:** Output signal resembles noise due to spreading  
- **Result:** DSSS signal successfully generated using simple message input  

<details>
<summary>View Part A Image Result</summary>

<p align="center">
<img src="Results/laboratory files 19/FIG 1.png" alt="DSSS Simple Message" width="600">
<img src="Results/laboratory files 19/fig 3.png" alt="DSSS Simple Message" width="600">
  
</p>

</details>

---

### Part B – Generating a DSSS Signal Using Speech
In this section, a **speech signal** was used as the message input. The speech waveform was multiplied by the spreading code to produce the DSSS signal.

The resulting waveform still appeared noise-like, but it carried the speech information within the spread spectrum signal.

- **Purpose:** Demonstrate DSSS using real-world audio signals  
- **Observation:** Spread-spectrum waveform carries speech information  
- **Result:** Speech successfully converted into DSSS format  

<details>
<summary>View Part B Image Result</summary>

<p align="center">
<img src="Results/laboratory files 19/fig 4.png" alt="DSSS Speech Signal" width="600">
  
</p>

</details>

---

### Part C – Using the Product Detector to Recover the Message
At the receiver, a **product detector** was used along with the same spreading code. The received DSSS signal was multiplied by the PN code to **despread** the signal.

After filtering, the original message signal was recovered.

- **Purpose:** Recover the original message from the spread signal  
- **Observation:** Product detector removes spreading effect  
- **Result:** Original message signal successfully reconstructed  

<details>
<summary>View Part C Image Result</summary>

<p align="center">
<img src="Results/laboratory files 19/fig 7.png" alt="DSSS Demodulation Using Product Detector" width="600">
<img src=" Results/laboratory files 19/fig 8.png" alt="DSSS Demodulation Using Product Detector" width="600">
</p>

</details>

---

### Part D – DSSS and Deliberate Interference (Jamming)
In this part, **deliberate interference (jamming)** was introduced into the DSSS system. The interference affected the transmitted signal, but due to the spreading technique, the system was able to reduce its impact.

After despreading using the correct PN code, the desired signal was recovered, while the interference was spread across the bandwidth.

- **Purpose:** Observe DSSS resistance to jamming  
- **Observation:** System maintains signal recovery despite interference  
- **Result:** DSSS demonstrates strong immunity to narrowband interference  

<details>
<summary>View Part D Image Result</summary>

<p align="center">
<img src="Results/laboratory files 19/fig 10.png" alt="DSSS Demodulation Using Product Detector" width="600">
<img src="Results/laboratory files 19/fig 11.png" alt="DSSS Demodulation Using Product Detector" width="600">
</p>

</details>

---

### Key Takeaways
- DSSS spreads the message signal using a **high-rate PN code**.
- The transmitted signal appears **noise-like** due to bandwidth spreading.
- A **product detector** is used to despread and recover the message.
- DSSS provides strong resistance against **interference and jamming**.
- This technique is widely used in modern wireless communication systems.
