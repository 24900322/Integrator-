## Experiment No: 4
INTEGRATOR USING OP-AMP (μA741)
## Aim
To design and simulate an Integrator circuit using μA741 in Proteus Design Suite and verify that the output is proportional to the integral of the input voltage.
## Apparatus Required
•	μA741 Op-Amp

•	Resistor R = 10 kΩ

•	Capacitor Cf = 0.01 µF

•	Signal Generator

•	Dual Power Supply (±15V)

•	CRO / Oscilloscope

•	Connecting wires
## Circuit Diagram
<img width="1919" height="1078" alt="image" src="https://github.com/user-attachments/assets/5008e11d-e599-438a-b38c-65546d622461" />

## Connection Details:
•	Input signal → Resistor (R) → Inverting terminal (Pin 2)

•	Feedback capacitor (Cf) → Between Output (Pin 6) and Pin 2

•	Non-inverting terminal (Pin 3) → Ground

•	Pin 7 → +15V

•	Pin 4 → −15V
## Theory
An Integrator circuit produces an output voltage proportional to the integral of the input voltage.
## Working Principle:
•	When input is constant → output is ramp signal

•	Output is inverted

•	Output depends on time

For Sine Wave Input:

•	Output lags input by 90°

•	Output amplitude decreases with frequency
## Procedure
1.	Open Proteus software.
2.	Select μA741, resistor, capacitor, signal generator, and CRO.
3.	Connect circuit in integrator configuration.
4.	Apply ±15V power supply.
5.	Set input waveform (1V, 1kHz).
6.	Run simulation.
7.	Observe input and output waveforms on CRO.
## Tabulation
## Observation Table – Integrator using µA741

| S.No | Input Signal | Frequency | Expected Output | Practical Observation |
|------|-------------|-----------|----------------|----------------------|
| 1 | Square Wave (±2.45 V) | 1 kHz | Triangular waveform | Small ramp waveform observed (≈ ±1.85 mV peak) |
| 2 | Sine Wave | 1 kHz | -Cosine wave (90° lag) | Phase-shifted sine wave (very low amplitude) |
| 3 | Triangular Wave | 1 kHz | Parabolic waveform | Slight curved waveform (low amplitude) |
## Waveforms
<img width="1380" height="893" alt="image" src="https://github.com/user-attachments/assets/72b79f2c-d851-4ea8-93ac-1d0b45d37d79" />

## Result
The Integrator circuit using μA741 Op-Amp was successfully designed and simulated in Proteus.
The output waveform is proportional to the integral of the input signal.
The circuit behaves as an integrator.
## Conclusion
•	Output lags input by 90° (for sine input).
•	Output amplitude decreases with increase in frequency.
•	Used in waveform generation and analog computation.
## Viva Questions

### 1. What is an integrator circuit?
An integrator is an op-amp circuit that produces an output proportional to the integral of the input signal.

---

### 2. Write the output equation of integrator.
Vout = - (1/RC) ∫ Vin dt

Where:
R = Input resistor  
C = Feedback capacitor  

---

### 3. Why does output lag input?
Because integration of a sine wave produces a -cosine wave, which lags the input by 90°.

---

### 4. What happens at very low frequency?
At very low frequency, gain becomes very high and the output may saturate due to DC components.

---

### 5. What is practical integrator?
A practical integrator is a modified integrator circuit with a resistor connected in parallel with the feedback capacitor to improve stability and reduce saturation.
