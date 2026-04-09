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
   ![WhatsApp Image 2026-04-09 at 8 35 32 AM](https://github.com/user-attachments/assets/80b27f18-4070-4fb4-a262-6fd2547ebfe9)

   ![WhatsApp Image 2026-04-09 at 8 35 45 AM](https://github.com/user-attachments/assets/3ae961c0-c9f5-40ab-8430-b7fc29dec0d4)


   

   __Tabulation__:
   <img width="864" height="1534" alt="image" src="https://github.com/user-attachments/assets/ce02b7b1-217f-4dd1-b20c-1eca5e00551b" />


   __Output__:
![WhatsApp Image 2026-04-09 at 8 36 27 AM](https://github.com/user-attachments/assets/e7e896f8-a46f-4171-bedd-f3fd2ff1d860)

   __Result__:
   ![WhatsApp Image 2026-04-09 at 8 35 54 AM](https://github.com/user-attachments/assets/af79fff7-2c8e-4fc5-a242-6d253603fce7)

