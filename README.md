# Acoustic Signal Localization Using Fourier Analysis

Tracking submarine motion from noisy acoustic data using Fourier analysis and FFT filtering.

## Overview

In this project, I use Fourier analysis and the Fast Fourier Transform (FFT) to analyze noisy three-dimensional acoustic data and track the motion of a submarine over time.

The original data is difficult to interpret because the submarine signal is mixed with a large amount of background noise. To make the data usable, I transform it into the frequency domain, where the dominant frequency associated with the submarine becomes much easier to identify.

After locating the dominant frequency, I apply a narrow-band Fourier filter to isolate the submarine signal and remove most of the noise. I then use the inverse Fourier transform to reconstruct the submarine trajectory in physical space over a 24-hour period.

This project demonstrates how Fourier-based methods can be used to recover meaningful structure from noisy high-dimensional data.

---

## Project Goals

The main goals of this project are to:

- identify the dominant acoustic frequency emitted by the submarine
- reduce noise using frequency-domain filtering
- reconstruct the submarine trajectory in 3D space
- analyze the resulting motion over time

---

## Methods

This project was implemented in Python using:

- NumPy
- Fast Fourier Transform (FFT)
- inverse FFT
- frequency-domain filtering
- data visualization

The workflow consists of:

1. transforming the acoustic data into Fourier space
2. averaging the frequency spectrum across time
3. identifying the dominant submarine frequency
4. applying a narrow-band filter around the dominant mode
5. reconstructing the filtered signal in physical space
6. tracking the submarine position over time

---

## Results

The Fourier filter successfully removed most of the background noise while preserving the submarine signal.

After reconstruction, the submarine appeared as a localized peak in space at each time step, making it possible to track its motion continuously over time.

The resulting trajectory is smooth and physically consistent, showing that Fourier-domain filtering is effective for identifying coherent structures in noisy data.

---

## Author

Hyo Jung Yoon  
University of Washington  
Applied & Computational Mathematics
