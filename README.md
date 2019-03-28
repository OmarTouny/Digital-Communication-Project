# Communication-Project

# General Instructions in all schemas:
### 1. Random Integer Generator
* Initial seed = 37
* Sample time = 0.1s
* Samples per frame = 100
### 2. AWGN Channel
* Initial seed = 67
* Number of bits per symbol = 1
* Input signal power = 1
* Symbol period = 1s
* Simulation time = 1000s
### 3.BER diagrams are set from -10 to 10 dB
------------------------------------------------------------------
# Quadrature Phase Shift keying Modulation

### QPSK can be stated as a method for transmitting digital information across an analog channel. Data bits are grouped into pairs, and each pair is represented by a particular waveform, called a symbol, to be sent across the channel after modulating the carrier. The most commonly used modulation scheme for wireless and cellular systems is Quadrature Phase Shift Keying (QPSK). It’s because it does not suffer from BER degradation while the band width efficiency is increased

## The modulation Schema contains: 
1.	The Random Integer Generator block, block generates uniformly distributed random integers in the range [0, M-1], where M is specified by the Set size parameter
2.	The QPSK Modulator Baseband block, to the right of the Integer Random Generator block, modulates the signal.
3. The Constellation Diagram block, displays a scatter plot of the signal without the added noise.
4.	The AWGN Channel block models a noisy channel by adding white Gaussian noise to the modulated signal.
5.	The Constellation Diagram block, displays a scatter plot of the signal with added noise.
6.	The QBSK Demodulator Baseband block Baseband block, to the right of the AGWN channel demodulates the signal.
7.	The Error Rate Calculation block counts symbols that differ between the received signal and the transmitted signal.
## The Modulation Schema
![QPSK](/QPSK/Scheme.png)
8.	The To Workspace block, labeled Ber outputs the results to the workspace to use when plotting results.
## Instruction SET:
* Random Integer Generator set size = 4
## Scatter Plot:
![Before Noise](/QPSK/BeforeNoise.png)

![After Noise](/QPSK/AfterNoise.png)

## BER performance figure:
![Error Curve](/QPSK/ErrorCurveQPSK.png)
------------------------------------------------------

# Frequency Shift Keying Modulation

### The FSK modulation is a digital modulation technique in which frequency of the carrier signal varies in accordance to the digital binary data (1 or 0). Binary logic-1 represents higher carrier frequency and logic-0 represents lower carrier frequency.

### The modulation Schema contains: 
1.	The Random Integer Generator block, block generates uniformly distributed random integers in the range [0, M-1], where M is specified by the Set size parameter
2.	The FSK Modulator Baseband block, to the right of the Integer Random Generator block, modulates the signal.
3. The Constellation Diagram block, displays a scatter plot of the signal without the added noise.
4.	The AWGN Channel block models a noisy channel by adding white Gaussian noise to the modulated signal.
5.	The Constellation Diagram block, displays a scatter plot of the signal with added noise.
6.	The FSK Demodulator Baseband block, to the right of the AGWN channel demodulates the signal.
7.	The Error Rate Calculation block counts symbols that differ between the received signal and the transmitted signal.
8.	The To Workspace block, labeled Ber outputs the results to the workspace to use when plotting results.
## The Modulation Schema
![FSK](/FSK/Scheme.png)
## Instruction SET:
* Random Integer Generator set size = 8
## Scatter Plot:
![Before Noise](/FSK/BeforeNoise.png)

![After Noise](/FSK/AfterNoise.png)

## BER performance figure:
![Error Curve](/FSK/ErrorCurveFSK.png)

------------------------------------------------------

# 16-Quadrature Amplitude Modulation
### quadrature amplitude modulation provides some significant benefits for data transmission one of them is 16 QAM

## The modulation Schema contains: 
1.	The Random Integer Generator block, block generates uniformly distributed random integers in the range [0, M-1], where M is specified by the Set size parameter
2.	The Rectangular QAM Modulator Baseband block, to the right of the Integer Random Generator block, modulates the signal using baseband 16 QAM.
3. The Constellation Diagram block, displays a scatter plot of the signal without the added noise.
4.	The AWGN Channel block models a noisy channel by adding white Gaussian noise to the modulated signal.
5.	The Constellation Diagram block, displays a scatter plot of the signal with added noise.
6.	The Rectangular QAM Demodulator Baseband block, to the right of the AGWN channel demodulates the signal.
7.	The Error Rate Calculation block counts symbols that differ between the received signal and the transmitted signal.
8.	The To Workspace block, labeled Ber outputs the results to the workspace to use when plotting results.
## The Modulation Schema
![QAM16 ](/QAM16/Scheme.png)
## Instruction SET:
* Random Integer Generator set size = 16

* Modulator and demodulation: Normalization method = Average power
## Scatter Plot:
![Before Noise](/QAM16/BeforeNoise.png)

![After Noise](/QAM16/AfterNoise.png)

## BER performance figure:
![Error Curve](/QAM16/ErrorCurveQAM16.png)

-----------------------------------------------------------
# 64-Quadrature Amplitude Modulation

###  quadrature amplitude modulation provides some significant benefits for data transmission one of them is 16 QAM

## The modulation Schema contains: 
1.	The Random Integer Generator block, block generates uniformly distributed random integers in the range [0, M-1], where M is specified by the Set size parameter
2.	The Rectangular QAM Modulator Baseband block, to the right of the Integer Random Generator block, modulates the signal using baseband 64 QAM.
3. The Constellation Diagram block, displays a scatter plot of the signal without the added noise.
4.	The AWGN Channel block models a noisy channel by adding white Gaussian noise to the modulated signal.
5.	The Constellation Diagram block, displays a scatter plot of the signal with added noise.
6.	The Rectangular QAM Demodulator Baseband block, to the right of the AGWN channel demodulates the signal.
7.	The Error Rate Calculation block counts symbols that differ between the received signal and the transmitted signal.
8.	The To Workspace block, labeled Ber outputs the results to the workspace to use when plotting results.
## The Modulation Schema
![QAM64](/QAM64/Scheme.png)
## Instruction SET:
* Random Integer Generator set size = 64

* Modulator and demodulation

Normalization method = Average power
## Scatter Plot:
![ Before Noise](/QAM64/BeforeNoise.png)

![ After Noise](/QAM64/AfterNoise.png)

## BER performance figure:
![Error Curve](/QAM64/ErrorCurveQAM64.png)

------------------------------------------------------------------

# Binary Phase Shift Keying Modulation

### Binary Phase Shift Keying (BPSK) is a type of digital modulation technique in which we are sending one bit per symbol i.e., ‘0’ or a ‘1’. Hence, the bit rate and symbol rate are the same. Depending upon the message bit, we can have a phase shift of 0 or 180 degree with respect to a reference carrier.

## The modulation Schema contains: 
1.	The Random Integer Generator block, block generates uniformly distributed random integers in the range [0, M-1], where M is specified by the Set size parameter
2.	The BPSK Modulator Baseband block, to the right of the Integer Random Generator block, modulates the signal.
3. The Constellation Diagram block, displays a scatter plot of the signal without the added noise.
4.	The AWGN Channel block models a noisy channel by adding white Gaussian noise to the modulated signal.
5.	The Constellation Diagram block, displays a scatter plot of the signal with added noise.
6.	The BPSK Demodulator Baseband block Baseband block, to the right of the AGWN channel demodulates the signal.
7.	The Error Rate Calculation block counts symbols that differ between the received signal and the transmitted signal.
8.	The To Workspace block, labeled Ber outputs the results to the workspace to use when plotting results.
## The Modulation Schema
![BPSK](/BPSK/Scheme.png)
## Instruction SET:
* Random Generator set size = 2
## Scatter Plot:
![Before Noise](/BPSK/BeforeNoise.png)

![After Noise](/BPSK/AfterNoise.png)

## BER performance figure:
![Error Curve](/BPSK/ErrorCurveBPSK.png)



---------------------------------------------------------------