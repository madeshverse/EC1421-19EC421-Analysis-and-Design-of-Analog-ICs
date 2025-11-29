# EC1421-19EC421-Analysis-and-Design-of-Analog-ICs
# DESIGN OF ACTIVE LOW PASS,HIGH PASS AND BAND PASS FILTERS USING OP-AMP 

## AIM: 

To design and obtain the frequency response of 
i) First order Low Pass Filter (LPF) 
ii) First order High Pass Filter (HPF) 
iii) Band pass filter
 
## APPARATUS REQUIRED

<img width="625" height="170" alt="image" src="https://github.com/user-attachments/assets/900fc8b3-3a8c-4208-bf52-98cc9e281e21" />

## THEORY
## LOW PASS FILTER 
 A LPF allows frequencies from 0 to higher cut of frequency, fH.  At fH the gain is 0.707 
Amax, and after fH gain decreases at a constant rate with an increase in frequency.  The gain 
decreases 20dB each time the frequency is increased by 10.  Hence the rate at which the gain 
rolls off after fH is 20dB/decade or 6 dB/ octave, where octave signifies a two fold increase in 
frequency.  The frequency f=fH is called the cut off frequency because the gain of the filter at this 
frequency is down by 3 dB from 0 Hz.  Other equivalent terms for cut-off frequency are -3dB 
frequency, break frequency, or corner frequency.
# HIGH PASS FILTER 
The frequency at which the magnitude of the gain is 0.707 times the maximum value of 
gain is called low cut off frequency.  Obviously, all frequencies higher than fL are pass band 
frequencies with the highest frequency determined by the closed –loop band width all of the op
amp. 
# BAND PASS FILTER 
A band pass filter has a pass band between two cutoff frequencies fH and fL such that fH > 
fL.  Any input frequency outside this pass band is attenuated.  There are two types of band-pass 
filters.  Wide band pass and Narrow band pass filters.  We can define a filter as wide band pass if 
its quality factor Q <10.  If Q>10, then we call the filter a narrow band pass filter.  A wide band 
pass filter can be formed by simply cascading high-pass and low-pass sections.  The order of 
band pass filter depends on the order of high pass and low pass sections.

## CIRCUIT DIAGRAM: 
## LOW_PASS


![WhatsApp Image 2025-11-29 at 10 36 46_f8187ccd](https://github.com/user-attachments/assets/b67b635d-fc19-40d3-a4cd-8b34a23efdb8)

## HIGH-PASS


![WhatsApp Image 2025-11-29 at 10 36 45_2bd38edc](https://github.com/user-attachments/assets/b2e1a8be-2c40-4efc-8d80-2ccbe3462bd3)


## BAND-PASS


![WhatsApp Image 2025-11-29 at 10 36 45_cfbfa865](https://github.com/user-attachments/assets/55a78b14-2e84-418b-be71-dfe86c14a667)


## MODEL GRAPH:
## LOW_PASS

![WhatsApp Image 2025-11-29 at 10 40 18_07482a6e](https://github.com/user-attachments/assets/e03d294c-06d6-4ab4-bd8a-8c34b1b469e2)

## HIGH-PASS


![WhatsApp Image 2025-11-29 at 10 40 37_a282ef8a](https://github.com/user-attachments/assets/d0865051-f201-40d5-a0b5-34a6ed4e8a48)


## BAND-PASS


![WhatsApp Image 2025-11-29 at 10 40 54_9a2e2044](https://github.com/user-attachments/assets/60e10a1b-3d48-488f-875d-bbe0e367dc9f)


## PROCEDURE - (LPF & HPF): 
1. Connect the circuit as shown in the circuit diagram. 
2. Select the corresponding cut-off frequency (higher or lower) and determine the value of C&R. 
select the value of R1 & Rf depending on desired passband gain Af.. 
3. Apply a constant voltage input sinusoidal signal to the non-inverting terminal of op-amp. 
4. Tabulate the output voltage Vo with respect to different values of input frequency. 
5. Calculate passband gain and plot the graph of frequency versus voltage gain & check the 
graph to  get approximately the same characteristic as shown in the model graph. 
# PROCEDURE:BAND PASS FILTER 
1. Select the lower and higher cut-off frequency and calculate the value of R & C for the given 
frequencies. 
2. Design for LPF & HPF separately and then combine the circuit by first placing the HPF 
followed by a LPF (i.e) HPF in series with LPF. 
3. Connect the circuit as shown in the circuit diagram. 
4. Apply a constant voltage input sinusoidal signal to the non-inverting terminal of op-amp. 
5. Tabulate the output voltage Vo with respect to different values of input frequency. 
6. Calculate passband gain and plot the graph of frequency versus voltage gain & check the 
graph to get approximately the same characteristic as shown in the model graph

## DESIGN:LPF & HPF:

<img width="429" height="324" alt="image" src="https://github.com/user-attachments/assets/b0f0ac0a-3006-494c-9096-e91ae2d6e87c" />

# DESIGN: BAND PASS FILTER
Design a BPF to pass a band of 400Hz to 2KHz with a pass band gain of 4.  
1. Select the highest cut-off frequency of LPF as fH = 10 KHz and the lowest cut-off frequency 
of HPF as fL = 1 KHz.  
2. Design the HPF first by taking fL = 1KHz. Assume the value of C < 1μf.  
Let C = 0.1μf.  
3. Calculate R from the expression.  
Given: fH = 2KHz  = 1/ (2πR1C1) 
   Let C1 = 0.1 µF, R1 = 7.9 KΩ 
Given: fL = 400Hz  = 1/ (2πR2C2) 
   Let C2 = 0.1 µF, R2 = 39.8 KΩ 
  Pass band Gain=4 
   Now   Ao = 1 + (Rf / R1)  
               2-1=(Rf / Ri) 
                Ri = Rf 
                 Let  Ri = Rf = 10 KΩ
## TABULATION:
## LOW_PASS


![WhatsApp Image 2025-11-29 at 10 42 18_936a2f9a](https://github.com/user-attachments/assets/e3c59690-75ed-47e3-a428-7eab23224397)


## HIGH-PASS


![WhatsApp Image 2025-11-29 at 10 42 19_06c65c7b](https://github.com/user-attachments/assets/ab53b900-4c19-48d3-a6a3-d23043d03e01)

## BAND-PASS


![WhatsApp Image 2025-11-29 at 10 43 11_7ecaa2cd](https://github.com/user-attachments/assets/83498da2-9deb-4bad-97b8-f78b4fb54152)


## GRAPH:
## LOW_PASS


![WhatsApp Image 2025-11-29 at 10 43 47_41774d29](https://github.com/user-attachments/assets/9d7f3907-acb6-437e-b04c-90321ada8a83)


## HIGH-PASS


![WhatsApp Image 2025-11-29 at 10 43 59_9ea00dfa](https://github.com/user-attachments/assets/10f2df38-3697-4e92-a16b-107e771537e2)


## BAND-PASS


![WhatsApp Image 2025-11-29 at 10 44 08_42272609](https://github.com/user-attachments/assets/91777edb-589b-447a-8a0c-577a40990e0b)


 ## RESULTS:
Thus an Active Low pass, High pass and Band Pass Filters are designed and 
tested using op-amp IC 741. 

