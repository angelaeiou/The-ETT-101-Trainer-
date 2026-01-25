# Part 3: Mathematical Equation Modeling Using the ETT 101 🧮

## Introduction

This experiment uses the Telecoms-Trainer 101 to demonstrate how mathematical equations can be modeled using analog signals. By interconnecting functional modules such as signal sources and adders, mathematical relationships between signals can be represented and observed in real time. This approach helps visualize abstract equations through measurable waveforms.

### Modeling of Equations

In this experiment, input signals are applied to different modules where each signal represents a variable in an equation. The contributions of each input are combined proportionally, allowing the output signal to represent the resulting equation. By adjusting signal amplitudes and phase relationships, constructive and destructive interference can be observed, showing how variables interact within the modeled equation. Observing the output waveform on the oscilloscope allows analysis of how changes in the inputs affect the final result, reinforcing the relationship between mathematical equations and physical signals.

#### Adder Module Concept 

The Adder module combines two input signals into a single output signal. Each input contributes proportionally to the final output based on its gain setting. Mathematically, it can be implemented using the Equation:
<p align="center">
  <em>Adder Module Output = Signal A + Signal B</em>
</p>

  <details>
    <summary><strong>Modeling Mathematical Equations Using an Adder Module</strong></summary>
  
   <p align="center">
      <img src="Results/laboratory files 2/Setups/Master Signals Block Diagram.jpeg" alt="Waveform Output" width="600">
    </p>
  <p align="center">
    <em>Figure 3.1: Adder Module Block Diagram</em>
  </p>
  
   <p align="center">
      <img src="Results/laboratory results part 3/Adder Setup.jpeg" alt="Waveform Output" width="600">
    </p>
  <p align="center">
    <em>Figure 3.2: Adder Module Setup</em>
  </p>

### Results
 <p align="center">
    <img src="Results/laboratory results part 3/Result 1.jpeg" alt="Waveform Output" width="600">
  </p>
<p align="center">
  <em>Figure 3.3: Adder Module Result in Oscillator</em>
</p>
The oscilloscope results show that when identical input signals are applied to the adder module, the output signal has approximately twice the peak-to-peak voltage of a single input. This confirms the adder modeling equation, where the output is equal to the sum of the input signals. The observed doubling of the output validates the theoretical expectation of linear signal addition.
</details>

####  Adder Module Output with Phase-Shifted Inputs
The Phase Shifter module changes the phase of an input signal without significantly affecting its amplitude. The amount of phase shift applied depends on the module’s control setting. By adjusting the phase, the relative timing between signals can be modified, allowing observation of constructive and destructive interference when phase-shifted signals are combined. This behavior is essential in signal alignment, modulation, and communication system analysis.

<p align="center">
  <em>Adder Module Output = Signal A + Signal B(with phase shift)</em>
</p>
<details>
    <summary><strong>Modeling Mathematical Equations Using a Phase Shifter Module</strong></summary>
  
   <p align="center">
      <img src="Results/laboratory results part 3/Adder With Phase Shift Block Diagram.jpeg" alt="Waveform Output" width="600">
    </p>
  <p align="center">
    <em>Figure 3.4: Adder Module with Phase Shifter Block Diagram</em>
  </p>
  
   <p align="center">
      <img src="Results/laboratory results part 3/Adder with Phase Shift Setup.jpeg" alt="Waveform Output" width="600">
    </p>
  <p align="center">
    <em>Figure 3.5: Adder Module with Phase Shifter Setup</em>
  </p>
### Results
 <p align="center">
    <img src="Results/laboratory results part 3/Result 2.jpeg" alt="Waveform Output" width="600">
  </p>
<p align="center">
  <em>Figure 3.6: Adder Module with Phase Shifter Result in Oscillator</em>
</p>
The oscilloscope shows the output of the adder module when two input signals with the same frequency and amplitude but a phase difference of approximately 90° are applied. Due to this phase shift, the signals do not fully add at all times, resulting in a combined waveform with a varying amplitude. This behavior confirms that the adder output depends on the phase relationship of the inputs, consistent with the theoretical summation of phase-shifted signals.​
