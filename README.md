# -Amplitude-Modulation-and-Demodulation-using-NumPy-and-Matplotlib

## Aim: 

To implement and analyze amplitude modulation (AM) using Python's NumPy and Matplotlib libraries. 

## Apparatus Required: 

Software: Python with NumPy and Matplotlib libraries 
Hardware: Personal Computer 

## Theory: 

Amplitude Modulation (AM) is a technique used in electronic communication, primarily for transmitting 
information via a radio carrier wave. In AM, the amplitude of the carrier wave is varied in proportion to that of 
the message signal. The general form of an AM signal is: 


## Algorithm:
1. Initialize Parameters: Set the values for carrier frequency, message frequency, and sampling frequency. 
2. Generate Time Axis: Create a time vector for the signal duration. 
3. Generate Message Signal: Define the message signal as a cosine wave. 
4. Generate Carrier Signal: Define the carrier signal as a cosine wave. 
5. Modulate Signal: Apply the AM formula to obtain the modulated signal. 
6. Plot the Signals: Use Matplotlib to plot the message signal, carrier signal, and modulated signal.

## Program:
```
import  numpy as np
import matplotlib.pyplot as plt
Am=8.5
fm=510
Ac=17
fc=5100
fs=51000
t=np.arange(0, 2/fm, 1/fs)

m=Am*np.cos(2*3.14*fm*t)
plt.subplot(3,1,1)
plt.plot(t,m)

c=Ac*np.cos(2*3.14*fc*t)
plt.subplot(3,1,2)
plt.plot(t,c)

s=(Ac+m)*np.cos(2*3.14*fc*t)
plt.subplot(3,1,3)
plt.plot(t,s)
```

 ## Output:
 <img width="567" height="413" alt="image" src="https://github.com/user-attachments/assets/bb18dd72-e15b-407c-8aa3-5d03572913c7" />

 ## Tabulation:
 ![WhatsApp Image 2025-11-23 at 15 42 50_b34616b1](https://github.com/user-attachments/assets/0932c32a-1aac-4ad0-9d34-d698fa5d02fe)

 ## Result:
 The AM experiment shows how the carrier amplitude varies according to the message signal, producing a modulated wave with carrier and sidebands. The output clearly displays both the envelope and frequency components, confirming successful modulation. The process helps understand how information is added to a carrier for simple and effective communication.


