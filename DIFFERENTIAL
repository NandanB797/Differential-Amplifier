# Differential-Amplifier
The report is about the differential amplifier with different configurations and analyzing the AC, DC and Transient analysis.


## CONTENTS:
* Introduction to Differential Amplifiers
* Working Principle of Differential Amplifiers
* Analysis & Design of Differential Amplifiers
* Circuit Design and Specifications
* LTSpice Simulation Steps
* Frequency Response & Gain Calculation
* Applications of Differential Amplifiers
* Simulation Results
* Inference
* Conclusion


# 1. Introduction to Differential Amplifiers
A differential amplifier is a key component in many analog circuits. Its primary role is to amplify the difference between two input signals, while filtering out any signals that are common to both inputs. This makes it highly effective in reducing noise and improving signal integrity. It’s used in a variety of applications, such as operational amplifiers (op-amps), sensor signal processing, and communication systems.

Operational Amplifier (Op-Amp) as Differential Amplifier

An operational amplifier can be used as a differential amplifier by connecting the two inputs to the non-inverting and inverting terminals of the op-amp. This is the most common configuration in practical applications.

The circuit typically consists of two main transistors (or MOSFETs) that work together to amplify the voltage difference between two input signals. The output of the amplifier is proportional to this difference.

In a simple equation: \[ V_out = A_d (V_1 - V_2) \]
 
Where 
V_out is the output voltage, V_1 and V_2 are input voltages and A_d is the differential gain.

# 2. Working Principle of Differential Amplifiers
Differential amplifiers function based on the following principles:

* They amplify only the difference between two input signals, rejecting any noise common to both inputs (common-mode signals).
* When both inputs are the same, the output should ideally be zero (i.e., no amplification).
* The key to good performance is having a high Common-Mode Rejection Ratio (CMRR), which ensures that common-mode signals are suppressed while differential signals are amplified.

# 3. Analysis & Design of Differential Amplifiers
* When designing a differential amplifier, it’s crucial to consider the common mode signal (when V_1 = V_2).
* The gain of the amplifier is determined by the relationship between the resistors and the transistor parameters. For example:
\[V_out = V_dd - I_d * R_d \]
 
Where:
* V_dd is the supply voltage,
* I_d is the current through the drain,
* R_d is the resistance in the drain circuit.
To maintain high performance, proper transistor selection and biasing are essential, as well as choosing appropriate resistor values to set the gain.

# 4. Circuit Design and Specifications:
Given:
Design and analyse the differential amplifier for the following specifications
V_dd = 1.8V, P <= 2.2mW, V_in_cm = 0.95 V, V_o_cm = 1.1V, V_p = 0.4V.
To perform the DC, AC, Transient Analysis for the above specifications.

Circuit diagram:
![ckt1](https://github.com/user-attachments/assets/6b377562-62ad-4e51-844c-d39eeebacc21)

Calculations:
To find the R_d, R_ss.
![image](https://github.com/user-attachments/assets/5cea4253-13b9-414e-b118-db8c24eb2e7d)

​

# 5. LTSpice Simulation Steps
   
Step 1: DC Analysis
* Set up the circuit in LTspice, including the MOSFET,resistors, and supply voltage (Vdd). change the name as CMOSN and give the length and width value. Use the .op command to perform the DC operating point analysis in LTspice. Check the DC values and operating points. Match the output values and current as per the given specifications and calculations.

Step 2: Transient Analysis 
* Add an AC signal source (Vin) at the gate of the MOSFET. Use the .tran command in LTspice for transient analysis. Set the simulation time and time step (e.g., 5ms). Observe the output waveform to measure the time-domain response, such as the output signal amplitude and phase shift.

Step 3: AC Analysis 
* Replace the DC signal source with an AC signal source (small AC voltage like 1V). Use the .ac command to perform frequency response analysis. Set the frequency range, e.g., from 1 Hz to 10 MHz, and analyze the magnitude and phase of the voltage gain. Observe the frequency response and note the gain and bandwidth.


# 6. Frequency Response & Gain Calculation
The gain of a differential amplifier is mainly dependent on the transconductance (g_m ) of the transistors and the load resistance. A simplified expression for the differential gain A_d is:

\[A_d = -g_m * R_d\]
 
Where g_m is the transconductance, which depends on the biasing conditions of the transistors.

The frequency response is influenced by factors like:
Bandwidth: The range of frequencies over which the amplifier can effectively amplify signals.

# 7. Applications of Differential Amplifiers
   
Differential amplifiers are used in:

Operational Amplifiers (Op-Amps): They form the basis of op-amps, which are used in a wide range of analog circuits.
Sensor Interfaces: Amplifying small signals from sensors while rejecting noise.
Instrumentation: Used in precision measurement systems.
Communication Systems: To enhance signal quality by removing noise.

# 8. Simulation Results 
Through simulations in LTSpice, various aspects of the differential amplifier can be observed:

* DC Analysis: Verifies that the transistors are operating in the active region.
* Transient Analysis: Shows how the circuit reacts to input signals over time, verifying amplification and stability.
* AC Analysis: Displays how the circuit performs across a range of frequencies, helping identify the bandwidth and frequency response.
 By replacing components like resistors with MOSFETs or current sources, we can improve gain, reduce power consumption, and enhance common-mode rejection. However, trade-offs may occur, such as reduced power efficiency when using MOSFETs in place of resistors.

## Circuit 1:
![ckt1](https://github.com/user-attachments/assets/6b377562-62ad-4e51-844c-d39eeebacc21)

## DC Analysis:
![op 1](https://github.com/user-attachments/assets/002c5b77-869e-4b1d-8e5c-66e04630a2a0)

## Transient Analysis:
![tr 1](https://github.com/user-attachments/assets/5edaf45c-58ec-48ac-beed-20870e16af6e)
![tr 11](https://github.com/user-attachments/assets/d53df214-da2f-46bb-b375-f208cf26eea3)
Vout = 1.719V

Av= 1.719 V/V

## AC Analysis:
![ac 1](https://github.com/user-attachments/assets/e93fc8e6-ad81-4615-a0fe-aa1db9520264)

3dB Gain = 19.548 dB

3dB gain bandwidth = 0 to 2.114 GHz

CMRR = Differential gain (gmRD) / Common mode gain (Vout/Vincm) = 11.37



## Circuit 2: 
Replacing Rss with Current Source Iss.
![ckt 2](https://github.com/user-attachments/assets/9898ff21-f3e4-4193-b89c-07bc0104ec5f)

## DC Analysis:
![op 2](https://github.com/user-attachments/assets/91d55f65-7a50-4b50-9e82-de0968791f1a)

 
## Transient Analysis:
![tr 2](https://github.com/user-attachments/assets/f389514e-43ac-42b7-aff8-da79b4126edf)
![tr 21](https://github.com/user-attachments/assets/0b93f6f4-f526-4596-8952-e95c5020d763)
![tr 22](https://github.com/user-attachments/assets/dcf2ea00-4c76-4ada-8c95-a1d6e5e43901)
Vout = 2.44V

Av = 1.742 V/V

 
## AC Analysis:
![ac 2](https://github.com/user-attachments/assets/44a08ea5-3f1e-49bc-abba-1b234912ad21)
3dB Gain = 19.54 dB

3dB gain bandwidth = 0 to 2.112 GHz

CMRR = Differential gain (gmRD) / Common mode gain (Vout/Vincm) = 11.21


## Circuit 3: 
Replacing Rss with NMOS and input V_b = 0.5V
![ckt 3](https://github.com/user-attachments/assets/961f1fee-02e5-443c-8c3c-615be7886457)


## DC Analysis:
![op 3](https://github.com/user-attachments/assets/069833e4-52b1-4192-8764-aa769a615cb5)

 
## Transient Analysis:
![tr 3](https://github.com/user-attachments/assets/7740e94f-bf6d-46ef-a17a-af39d682d47c)
![tr 31](https://github.com/user-attachments/assets/2ca0b03a-228a-4dad-9075-290b08d72fca)
Vout = 1.709V

Av = 1.709 V/V


## AC Analysis:
![ac 3](https://github.com/user-attachments/assets/d2d0b31d-92e8-4ef0-bbe2-19a5396501c8)
3dB Gain = 19.447 dB

3dB gain bandwidth = 0 to 2.127 GHz

CMRR = Differential gain (gmRD) / Common mode gain (Vout/Vincm) = 11.01



## Circuit 4: 
Replacing R_d1 amd R_d2 by PMOS.
![ckt 4](https://github.com/user-attachments/assets/893e6b1f-7173-4fa0-8ad0-b05278bc4268)

## DC Analysis:
![op 4](https://github.com/user-attachments/assets/ccccc346-54b5-407b-b4b1-a639ca5e9ded)

 
## Transient Analysis:
![tr 4](https://github.com/user-attachments/assets/6cc33d22-11d3-4d23-921f-079b00cda445)
![tr 41](https://github.com/user-attachments/assets/cacdbe6f-4b07-4b70-9aa6-546060febf19)
Vout = 337.8mV

Av = 1.876 V/V


## AC Analysis:
![ac 4](https://github.com/user-attachments/assets/dc04c930-e253-418a-a0ab-c61c78191bc5)
3dB Gain = 5.15 dB

3dB gain bandwidth = 0 to 5.75 GHz

CMRR = Differential gain (gmRD) / Common mode gain (Vout/Vincm) = 2.74


# 9. Inference
* M1 and M2 are identical MOSFETs and they are in saturation region.
* When Rss was replaced by current source Iss of 1.2mA, there is a bit difference in the operating point.
* Noise cancelation which is CMRR is the difference of input signals by cancelling the common mode signals.
* From Transient analysis we get the Vout peak to peak voltage to calculate the gain.
* We get high gain when we set AC phase as 180.

* 
# 10. Conclusion
The differential amplifier is a fundamental circuit in analog electronics, providing excellent signal amplification while rejecting noise. With proper design and component selection, it can achieve high gain, low noise, and superior common-mode rejection. Its versatility and effectiveness make it indispensable in modern analog systems such as op-amps, instrumentation, and communication systems. The simulation results demonstrate the amplifier’s ability to perform efficiently across a range of conditions, confirming its role as a key building block in electronics.

By leveraging MOSFETs and current sources, the design can achieve improved performance in terms of gain and noise rejection, making it suitable for advanced analog applications.
