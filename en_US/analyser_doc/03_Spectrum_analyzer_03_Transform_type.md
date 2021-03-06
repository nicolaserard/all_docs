# Transform type
The discrete Fourier transform (DFT) is the traditional method employed to compute the frequency
spectrum of a discrete digital signal. DFT can be seen as a series of notch filters centered around
frequency bins that are uniformly distributed along the frequency axis, and of constant width.

The quality factor of a resonant filter, commonly denoted as Q, is defined as the ratio of its bandwidth
relative to its center frequency. The DFT process is therefore analogous to a variable Q filter-bank, in
other words, its frequency resolution is constant across the spectrum. When applied to sliding blocks,
this process is called STFT, for Short-term Fourier transform.

Although convenient in terms of computation, this can be seen as less than ideal for many audio
applications, for several reasons, the first and foremost being that human perception of frequency is
known to be quasi-<i>logarithmic</i>. Logarithmic means that a two-fold increase in frequency translates
to a one octave shift, a four-fold increase as a two-octave shift - and not four as this would be the
case, were our perception linear in nature.

Pure Analyzer employs both standard DFT and proprietary algorithms that more closely model the human
perception. In addition to greatly improving the legibility of the resulting curves, this proprietary
transform has the additional benefit of reducing sensitivity to noise in the high-frequency portion of
the spectrum especially, and provides more stable readouts.

> You can of course switch back to standard DFT by disengaging the Pure spectrum button.

