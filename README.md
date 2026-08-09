# EXPT 1b: Computation-of-DFT-using-FFT-ALGORITHM

## AIM
To perform and verify DFT using FFT-ALGORITHM by SCILAB.
## APPARATUS REQUIRED
PC installed with SCILAB
## PROGRAM 
### DFT FFT-ALGORITHM
<br>clear;
<br>clc;
<br>close;
<br>xn = [1 2 3 4 4 3 2 1]
<br>n1=0:1:length(xn)-1;
<br>subplot(2,2,1);
<br>plot2d3(n1,xn);
<br>xlabel('Time n');
<br>ylabel('Amplitude');
<br>title('Input Sequence');
<br>Xk = fft(xn); 
<br>K1=0:1:length(Xk)-1;
<br>magnitude=abs(Xk)
<br>subplot(2,2,2);
<br>plot2d3(K1,magnitude);
<br>xlabel('frequency(Hz)');
<br>ylabel('magnitude(gain)');
<br>title('magnitude spectrum');
<br>angle = atan(imag(Xk),real(Xk))
<br>subplot(2,2,3);
<br>plot2d3(K1,angle);
<br>xlabel('frequency(Hz)');
<br>ylabel('Phase');
<br>title('Phase spectrum')
<br>y= ifft(Xk)
<br>n2=0:1:length(y)-1;
<br>subplot(2,2,4)
<br>plot2d3(n2,y)
<br>xlabel('Time n');
<br>ylabel('Amplitude');
<br>title('Inverse FFT OF X(K)');

<br>
**CALCULATIONS:**
<br> <img width="820" height="1339" alt="image" src="https://github.com/user-attachments/assets/e5d3ad7b-4867-47f7-96d8-70e124f5d6d5" />


**SAMPLE OUTPUT:**
<br> <img width="912" height="723" alt="image" src="https://github.com/user-attachments/assets/b0140bed-aa91-4bbb-8039-8780ef007c2e" />





## RESULT:
Thus,  DFT using FFT-ALGORITHM for two given sequences were performed and its result was verified.

