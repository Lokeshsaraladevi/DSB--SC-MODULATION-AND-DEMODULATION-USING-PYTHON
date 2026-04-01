# DSB--SC-MODULATION-AND-DEMODULATION-USING-PYTHON

__AIM__:

To generate a Double Sideband Suppressed Carrier (DSB-SC) signal in Python (Google Colab), transmit it (optionally add noise), and recover the message using coherent (synchronous) demodulation with a low-pass filter. Observe time and frequency domain waveforms and measure demodulation performance

__APPARATUS REQUIRED__:

Google Colab (or any Python environment)

Python libraries: numpy, matplotlib, scipy (scipy.signal)

__Theory__:

DSB-SC signal: s(t) = m(t) · cos(2πf_c t)
Coherent demodulation: multiply received s(t) by a synchronized carrier cos(2πf_c t) then low-pass filter (LPF) to remove double-frequency components:

r(t) = s(t)·cos(2πf_c t) = m(t)·cos²(2πf_c t) = 0.5 m(t) + 0.5 m(t)·cos(4πf_c t)
LPF extracts 0.5·m(t) → scale by 2 to recover m(t).

__Procedure__:

1) Import libraries and set parameters
2) Define message and carrier signals
3) Generate DSB-SC signal (modulation)
4) View spectra (FFT) of message and DSB-SC
5) (Optional) Add noise
6) Coherent demodulation (multiply by synchronized carrier)
7) Low-pass filter to recover message

 __Program__:
 
![WhatsApp Image 2026-04-01 at 7 26 21 AM](https://github.com/user-attachments/assets/ae195a18-4ded-4552-98b3-85c6da50cbd5)
![o](https://github.com/user-attachments/assets/c9893e0a-29f0-4992-b8ce-da0b91afab0e)

   
 __Tabulation__:
   
![p](https://github.com/user-attachments/assets/a5fdcfb3-099a-4388-a537-db94d3a5c1e8)

   __Output__:
   
![WhatsApp Image 2026-04-01 at 7 26 43 AM](https://github.com/user-attachments/assets/011f3c1e-59c2-49f7-abe8-3b2813744d04)

   __Result__:
   
   <img width="581" height="338" alt="image" src="https://github.com/user-attachments/assets/7c492b0a-a864-4954-b708-0ad92f92344f" />

