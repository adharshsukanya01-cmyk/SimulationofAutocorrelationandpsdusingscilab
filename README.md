# EXPT.NO.6	SIMULATION OF AUTOCORRELATION AND PSD USING SCILAB AIM:
Write a program for Autocorrelation and PSD of signals in SCILAB and verify Wiener-Khinchin relation.

# EQUIPMENTS Needed

*Computer with i3 Processor

*SCI LAB

# THEORY:
The Wiener-Khinchin theorem states that the power spectral density of a wide sense stationary random process is the Fourier transform of the corresponding autocorrelation function.

# Algorithm
1.Load or Define the Signal: Input your time-domain signal.

2.Compute Autocorrelation: Calculate the autocorrelation function of the signal.

3.Compute Power Spectral Density (PSD): Estimate the PSD of the signal, either directly using a method like Welch’s periodogram or by using the Fourier transform of the autocorrelation.

4.Plot Results: Visualize the autocorrelation function and PSD.

# PROCEDURE

Refer Algorithms and write code for the experiment.

Open SCILAB in System

Type your code in New Editor

Save the file

Execute the code

If any Error, correct it in code and execute again

Verify the generated waveform using Tabulation and Model Waveform



# PROGRAM:

clc

clear all;

t=0:0.01:2*3.14;

x=sin(10*t)+cos(10*t);

subplot(3,2,1);

plot(x);

au=xcorr(x);

subplot(3,2,2);

plot(au);

v=fft(au);

subplot(3,2,3);

plot(abs(v));

fw=fft(x);

subplot(3,2,4);

plot(fw);

fw2=(abs(fw))^2;

subplot(3,2,5);

plot(fw2);


# OUTPUT:

<img width="1920" height="1080" alt="Screenshot 2025-10-08 093804" src="https://github.com/user-attachments/assets/1d77f5b9-834f-47bb-954e-aadde3c84285" />
![298c352b-81fd-4273-8822-f55d0b382a82](https://github.com/user-attachments/assets/436fd0f9-9657-47e9-a48d-e00fc39e1e8b)
![f39a5a01-7bdf-4ee3-a0ff-68280eaf9f99](https://github.com/user-attachments/assets/29ae950a-85cc-41d1-aa3a-a6a8a842db5b)





# RESULT:
Thus the Autocorrelation and PSD are executed in Scilab and output is verified.
