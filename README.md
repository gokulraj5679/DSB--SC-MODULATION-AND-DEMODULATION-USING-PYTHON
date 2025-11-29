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

   __Tabulation__:
   ![WhatsApp Image 2025-11-29 at 10 26 14_d241c05f](https://github.com/user-attachments/assets/f79eea57-a195-4083-84d8-8413f5e5ec3b)
   ![WhatsApp Image 2025-11-29 at 10 26 30_def9c36b](https://github.com/user-attachments/assets/1fac02b3-66ae-43e7-91ec-9c64fb2bbfb6)






   __Output__:
<img width="989" height="590" alt="image" src="https://github.com/user-attachments/assets/4e00e5b8-9832-4091-8037-ed6221b3206b" />

   __Result__:
![WhatsApp Image 2025-11-29 at 10 26 30_def9c36b](https://github.com/user-attachments/assets/69fb664d-d117-41aa-a042-d515022a3c37)
