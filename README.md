"DIFFERENTIAL AMPLIFIER"
A differential amplifier is a fundamental building block in analog cicuit design, widely used in applications such as signal 
amplification, noise reduction and data acquisition systems.It amplifies the difference between two  input signal while rejecting 
common-mode noise,making it ideal for high-precision circuits including operational amplifiers and analog front end systems.


Q: VDD=1.8V,P<=2.2mW,VICM=0.95V,VOCM=1.1V,Vp=0.4V

CIRCUIT 1: 
![ckt1](https://github.com/user-attachments/assets/1362e14b-e262-46eb-b03f-3938f7a300f5)







STEP 1: Dc analysis
![n1](https://github.com/user-attachments/assets/b34ef8cb-3d3a-41d4-89d6-e0341a649ecf)

from above
Iss=1.3mA
Id=0.61mA
Rd=1.16kohm
Rss=333ohm
Vgs = vg-vp = 0.95-0.4=>0.55v
Vov=vgs-vth = 0.55-0.366 => 0.184

To set the operating point go to Configure Analysis and select Dc operating Point




Effect of VICM on Vout and VP




As the common-mode input voltage ( VICM ) increases, the source voltage ( VP ) also increases,
causing a shift in the operating point. This leads to a higher drain current, resulting
in a greater voltage drop across ( RD ), which reduces ( Vo

MAXIMUM I/P AND O/P SWING
![n2](https://github.com/user-attachments/assets/8f189ce0-01d1-4a8b-8cd5-e866509ae3e1)


GAIN
![n3](https://github.com/user-attachments/assets/dbc28754-0cd6-4d63-8092-2818925f39ed)

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
