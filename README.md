# SSB-T1-C12-EVEN
AIM:

To write a program for mean, variance and cross correlation in SCILAB and verify the output.

EQUIPMENTS NEEDED:

.Computer with i3 Processor

.SCI LAB

ALGORITHM:

Define the Function: Specify the function you want to simulate. For example, f(x)=sin⁡(x)f(x)=sin(x) or any other function.
Generate Sample Points: Decide on the range and the number of sample points. Generate these sample points within the desired range.
Evaluate the Function: Compute the function values at each of these sample points.
Compute Mean, Variance and Cross Correlation: Use Scilab's functions to calculate the mean and variance of the computed function values.
Display Results: Output the computed mean variance and Cross Correlation
PROCEDURE:

1.Refer Algorithms and write code for the experiment.

2.Open SCILAB in System

3.Type your code in New Editor

4.Save the file

5.Execute the code If any Error, correct it in code and execute again

6.Verify the generated results

PROGRAM:
```
clc;
clear;
close;

// Parameters
Am = 3.1;        // Message amplitude
Ac = 6.2;        // Carrier amplitude
fm = 146;      // Message frequency (Hz)
fc = 1460;     // Carrier frequency (Hz)
fs = 14600;    // Sampling frequency (Hz)

// Time vector
t = 0:1/fs:0.05;

// Message signal
m = Am * sin(2*%pi*fm*t);

// Carrier signal
c = Ac * sin(2*%pi*fc*t);

// SSB-SC modulation
ssb_sc = m .* c;

// Plotting
subplot(3,1,1)
plot(t, m)
title("Message Signal")
xlabel("Time")
ylabel("Amplitude")

subplot(3,1,2)
plot(t, c)
title("Carrier Signal")
xlabel("Time")
ylabel("Amplitude")

subplot(3,1,3)
plot(t, dsb_sc)
title("SSB-SC Modulated Signal")
xlabel("Time")
ylabel("Amplitude")
```
Tabulation:

![850a22d6-dfb0-4917-a48e-82845554c4cf](https://github.com/user-attachments/assets/4c72a328-cef5-4214-8d59-b06e62920ac5)

OUTPUT GRAPH:

<img width="1913" height="1199" alt="Screenshot 2026-02-14 114016" src="https://github.com/user-attachments/assets/a9cb40f8-474a-4d42-9879-b33389fe8497" />

RESULT:
Thus the SSB-SC-AM Modulation and Demodulation is generated.


