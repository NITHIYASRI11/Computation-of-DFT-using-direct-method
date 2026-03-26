# EXPT 1: Computation-of-DFT-using-direct-method

## AIM
To perform and verify DFT using direct method by SCILAB.
## APPARATUS REQUIRED
PC installed with SCILAB
## PROGRAM 
### DFT DIRECT METHOD
```
clear;
clc;
close all;
xn = [1 2 3 4 4 3 2 1];
n1 = 0:1:length(xn)-1;
subplot(2,2,1);
plot2d3(n1, xn);
xlabel('Time n');
ylabel('Amplitude');
title('Input Sequence');
Xk = fft(xn);
K1 = 0:1:length(Xk)-1;
magnitude = abs(Xk);
subplot(2,2,2);
plot2d3(K1, magnitude);
xlabel('Frequency (Hz)');
ylabel('Magnitude (gain)');
title('Magnitude Spectrum');
angle = atan2(imag(Xk), real(Xk));
subplot(2,2,3);
plot2d3(K1, angle);
xlabel('Frequency (Hz)');
ylabel('Phase');
title('Phase Spectrum');
y = ifft(Xk);
n2 = 0:1:length(y)-1;
subplot(2,2,4);
plot2d3(n2, y);
xlabel('Time n');
ylabel('Amplitude');
title('Inverse FFT of X(k)');
```
## CALCULATIONS:

<img width="1026" height="1599" alt="image" src="https://github.com/user-attachments/assets/db258ea3-cc3f-4e21-91d0-e213364a0adf" />
<img width="1545" height="1004" alt="image" src="https://github.com/user-attachments/assets/27fc0384-d951-47c8-9ba9-d23439b9a1b3" />

## SAMPLE OUTPUT:
![WhatsApp Image 2026-03-26 at 13 36 43](https://github.com/user-attachments/assets/c7dd5623-a9f8-4403-83a7-00ce8d012659)




## RESULT:
Thus,  DFT using direct method for two given sequences were performed and its result was verified.

