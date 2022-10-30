# Highlights of Spectral Analysis.

1. Foundamentals of Fourier transform;
2. Discrete Fourier Transform;
3. FFT to calculate DFT;
4. How to calculate FFT with python?
5. What is a periodogram and power spectral density (PSD)? 
6. PSD and FFT.
7. How to detect the harmonics of the signal automatically?

## Fourier Transform.

In spectral analysis or frequency-domain analysis, we study the frequencies or energies in the signal with the help of algorithms to estimate these components. The foundamentals start with the representation of periodic functions with the Fourier series. Any periodic signal in both continuous-time and discrete-time can be written as a sum of trigonometric functions, the sine-cossine form:

$$x[n] = \frac{a_0}{2} + \sum_{k=1}^N a_k cos(wkn) + b_k sin(wkn)$$

Another equivalent form, useful for this work, is shown below as the sum of complex exponentials with coeficients, with fundamental period N.

$$x[n] = \sum_{k=<N>} a_k e^{j w_0 n}$$
$$w_0 = \frac{2\pi}{N}$$

The coeficient $w_0$ marks the spacing between the frequencies and the $a_k$ can be obtained with:

$$a_k = \frac{1}{N} \sum_{n=<N>} x[n] e^{-jk(2\pi/N)n}$$

These two equations specify the decomposition of the original signal in a sum of N related exponentials. The coeficients $a_k$, in turn, maps how a particular frequency is important to the whole signal.

However, the development that envolves a broad range of applications are the Fourier transforms, because it deals with aperiodic signals which are present in most of the real-life systems. For an aperiodic sequence $x[n]$ in the discrete-time domain, $X(e^{jw})$ is defined as the discrete-time Fourier transform (DTFT) with the equation below.

$$X(e^{jw}) = \sum_{n=-\inf}^{+\inf}x[n]e^{-jwn}$$

The contribuition from each sample of the signal for the specified frequency $w$ gives the DTFT or the spectrum value for that frequency.
The oposite equation to form each element of the sequence is:

$$x[n] = \frac{1}{2\pi}\int_{2\pi}X(e^{jw})e^{jwn}dw$$

Many text books develop the Fourier transform of an aperiodic sequence by viewing that this sequence is periodic with a too long period, $N-> \inf$. This approach results in integrating the DTFT elements over the frequencies and shows one of the differences between the discrete and continuous-time signals: If a signal is discrete in the time-domain, it is continuous in the frequency-domain.

## Discrete Fourier transform (DFT).

So far, equations for the DTFT involves infinite sequences although aperiodic and continuous in frequency-domain. It's an improvement but, in practice, all applications in digital signal processing require to compute finite signals in the time and frequency-domain, represented by a limited number of samples. For those signals, an adaptation of the theory is made with the discrete Fourier transform (DFT).

Discrete-time signals can be viewed as sampled data from continuous-time phenomena, as the measurement of a current in a circuit. 

To recover a finite signal $x[n]$ it is not necessary to know $X(e^{jw})$ at all frequencies if the sequence has a finite length. Given a finite-length sequence $x[n]$, we can form a periodic sequence by the convolution with a sequence of pulse trains. Conversely, given a sequence of Fourier coefficients $X^~[k]$, we can find a periodic sequence $x^~[n]$ and recover $x[n]$ by taking one period. This is, in fact, what is happening when we are dealing with finite signals and trying to represent them with a finite sequence of Fourier coefficients in the DFT.

## FFT to calculate DFT
## How to calculate FFT with Python? (explain the normalization of FFT)
## What is a periodogram and power spectral density (PSD)? 
## PSD and FFT.
