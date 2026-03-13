# PCM Decoding Experiment

---

### Abstract
This experiment focused on the **decoding process of Pulse Code Modulation (PCM)** using the EMONA telecommunications trainer. The objective was to understand how digital PCM data can be converted back into an analog signal. By configuring the PCM encoder, decoding the PCM bit stream, and transmitting speech signals through the system, the experiment demonstrated the full process of **analog-to-digital and digital-to-analog signal conversion**. The results highlight the importance of proper synchronization, decoding, and filtering in digital communication systems.

---

### Introduction
Pulse Code Modulation (PCM) is widely used in digital communication systems to convert analog signals into digital form for transmission and storage. However, once the signal reaches the receiver, the digital data must be **decoded and reconstructed** in order to recover the original analog signal.

PCM decoding involves converting the binary data back into **quantized voltage levels**, which are then smoothed using a **reconstruction filter** to produce a continuous waveform. This process is fundamental in applications such as **digital telephony, audio playback systems, and digital broadcasting**.

---

### Theoretical Background
In a PCM system, the analog signal is first **sampled, quantized, and encoded** into a digital binary sequence. During decoding, the reverse process occurs:

1. **Digital Decoding** – The binary code is interpreted to determine the quantized amplitude level.
2. **Digital-to-Analog Conversion (DAC)** – The quantized digital value is converted into a corresponding voltage level.
3. **Reconstruction Filtering** – A low-pass filter smooths the staircase waveform to approximate the original analog signal.

Although the reconstructed signal closely resembles the original waveform, small differences may occur due to **quantization errors and sampling limitations**.

---

# Discussion

---

### Part A – Setting Up the PCM Encoder
In this part, the PCM encoder was configured to convert the input analog signal into a **binary digital representation**. The encoder samples the input signal and assigns each sample to a quantization level before converting it into a binary code.

- **Purpose:** Prepare the system to generate PCM data from an analog signal  
- **Observation:** Output consists of a sequence of binary pulses representing the input voltage  
- **Result:** A digital PCM data stream was successfully generated

<details>
<summary>View Part A Image Result</summary>

<p align="center">
<img src="Results/laboratory files 13/FIGURE 2.png" alt="PCM Encoder Setup" width="600">
<img src="Results/laboratory files 13/FIGURE 3.png" alt="PCM Encoder Setup" width="600">
 </p>

</details>

---

### Part B – Decoding the PCM Data
In this section, the PCM bit stream was passed into the **PCM decoder**, which interpreted the binary codes and converted them back into their corresponding quantized voltage levels.

The output signal appears as a **staircase waveform**, where each step corresponds to a decoded quantization level.

- **Purpose:** Convert PCM digital data back into analog voltage levels  
- **Observation:** Output waveform shows discrete voltage steps  
- **Result:** The binary PCM data was successfully decoded into an analog signal

<details>
<summary>View Part B Image Result</summary>

<p align="center">
<img src="Results/laboratory files 13/FIGURE 4.png" alt="PCM Decoder Output" width="600">
</p>

</details>

---

### Part C – Encoding and Decoding Speech
In this part, a **speech signal** was applied to the PCM encoder. The speech waveform was first encoded into digital PCM data and then passed through the decoder.

This demonstrated how real-world analog signals such as **human voice** can be transmitted digitally and reconstructed at the receiver.

- **Purpose:** Demonstrate PCM operation with complex signals such as speech  
- **Observation:** PCM data stream varies according to speech amplitude  
- **Result:** Speech signal was successfully encoded and decoded

<details>
<summary>View Part C Image Result</summary>

<p align="center">
<img src="Results/laboratory files 13/fig 5.png" alt="PCM Speech Encoding and Decoding" width="600">
<img src="Results/laboratory files 13/fig 10.png" alt="PCM Speech Encoding and Decoding" width="600">

</p>

</details>

---

### Part D – Recovering the Message
In the final stage, the decoded signal was passed through a **reconstruction filter** to smooth the staircase waveform and recover the original message signal.

The resulting waveform closely resembled the original analog input, demonstrating successful PCM communication.

- **Purpose:** Recover the original analog message from PCM data  
- **Observation:** Output waveform becomes smooth after filtering  
- **Result:** The reconstructed signal closely matches the original message signal

<details>
<summary>View Part D Image Result</summary>

<p align="center">
<img src="Results/laboratory files 13/FIGURE 2.png" alt="Recovered Analog Signal" width="600">
</p>

</details>

---

### Key Takeaways
- PCM decoding converts **digital binary data back into analog voltage levels**.
- The decoded signal initially appears as a **staircase waveform**.
- A **reconstruction filter** is used to smooth the signal and recover the original message.
- PCM systems enable reliable transmission of **audio, speech, and other analog signals** in digital form.
