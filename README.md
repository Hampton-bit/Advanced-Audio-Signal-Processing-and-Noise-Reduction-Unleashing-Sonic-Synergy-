# Advanced Audio Signal Processing and Noise Reduction
*Unleashing Sonic Synergy through Harmonic Resonance*

**Presented to:**  
Dr. Ahmad Salman  

**Presented by:** 
- M. Hamza Naeem (335797)  
- Wahab Hassan Janjua (341658)  
- Fahad Arshad (331804)  


## Introduction
This project explores various signal processing techniques applied to audio signals, focusing on spectral analysis, filtering, noise reduction through adaptive filters (specifically the LMS algorithm), voice activity detection (VAD), and volume control via a graphical user interface (GUI).

## Methodology
Implemented in **MATLAB**, the project follows these steps:

1. **Reading and Preprocessing the Audio Signal**:  
   The audio file (GGG.WAV) is read and converted from stereo to mono.

2. **Spectral Analysis**:  
   The sample rate is displayed, and the spectrogram and power spectral density of the audio signal are plotted.

3. **Fourier Transform**:  
   The Fourier transform is calculated to visualize frequency components and bandwidth.

4. **Filter Design and Application**:  
   Various filters (low-pass, high-pass, bandpass, and bandstop) are designed and applied to the audio signal, with the occupied bandwidth plotted.

5. **Noise Removal**:  
   White noise is added, and an adaptive LMS filter is used to remove the noise, with results shown in a spectrogram.

6. **Voice Activity Detection (VAD)**:  
   The short-term energy of the signal is calculated to detect speech versus silence, resulting in a binary output.

7. **Volume Control**:  
   A GUI is created to control audio volume, allowing users to adjust playback levels via a slider.

## Code Overview
- **Reading the Audio**: `y = audioread('GGG.WAV');`
- **Spectrogram Plotting**: `specgram(y, length(y), Fs);`
- **Filter Design**: Filters are designed using `fdesign` and `design` functions.
- **Adaptive Noise Filtering**: Implemented with `dsp.LMSFilter`.
- **Volume Control Function**: Adjusts playback volume dynamically based on user input.

## Conclusion
This project successfully demonstrates the application of advanced audio signal processing techniques, effectively enhancing audio quality through filtering, noise reduction, and user-controlled volume adjustment.
