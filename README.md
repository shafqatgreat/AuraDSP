# AuraDSP | Professional Audio Restoration Suite

![Main Interface](assets/1.AuraDSP.png)
**AuraDSP** is a standalone, high-performance audio restoration workstation designed for professional-grade noise suppression and signal recovery. Engineered for broadcast, podcasting, and forensic audio applications, AuraDSP utilizes proprietary spectral subtraction algorithms to isolate voice transients from complex background environments.

---

## 💎 Core Technologies

* **Spectral Subtraction V2 Engine:** Precision frequency-domain attenuation that identifies and eliminates stationary noise (hiss, hum, fan noise) with minimal artifacting.
* **Intelligent Monitoring Matrix:** Toggle-switch monitoring allows for real-time auditing of:
    * **Master Out:** The fully restored signal.
    * **Noise Delta:** The isolated noise profile being removed (Critical for precision calibration).
    * **Input Bypass:** The raw, unprocessed source.
* **Aura-Visualize Rendering:** A high-speed visualization engine capable of rendering both **Time-Domain Waveforms** and **Spectral Heat Maps** (Spectrograms).
* **Advanced Mastering Chain:**
    * **Sub-Sonic Filtration:** Integrated 5th-order high-pass cut at 80Hz.
    * **Transient Pre-emphasis:** Phase-aligned high-frequency boost for vocal clarity.
    * **Soft-Knee Limiter:** Non-linear amplitude management to ensure 0dBFS peak normalization without digital clipping.

---

## 📊 Engineering Specifications

The AuraDSP engine operates on a high-resolution analysis window to ensure surgical transparency.

| Architecture Component | Specification |
| :--- | :--- |
| **Analysis Window** | 2048-sample STFT |
| **Overlap Processing** | 75% (512-sample step) |
| **Filter Topology** | 5th-Order Butterworth |
| **Recovery Logic** | Tanh-based Soft Clipping |
| **Dynamic Range** | 24-bit / 32-bit Float Support |
| **Sampling Rate** | Native Multi-rate Support (Automatic Resampling) |



---

## 🖥️ Professional Visualization Modes

### Waveform Analysis Mode
High-precision amplitude tracking used to monitor signal dynamics and peak-to-average ratios. Perfect for ensuring consistent loudness levels across different recordings.


[Image of an audio waveform]


### Spectral Analysis Mode (TFT)
A top-tier frequency heat map that visualizes the "Aura" of the audio. Allows engineers to see hidden frequency interference, such as 50/60Hz electrical hum or high-frequency digital whine, and target it via the Reduction Strength slider.


[Image of an audio spectrogram]


---

## 📦 Deployment & Installation

### Standalone Binary
AuraDSP is distributed as a single-file, zero-dependency executable. No external runtimes or installations are required.

1. **Download:** Navigate to the **[Releases](https://github.com/yourusername/AuraDSP/releases)** tab.
2. **Execute:** Run `AuraDSP.exe`.
3. **Hardware:** Compatible with standard Windows 10/11 ASIO and WDM drivers.

---

## 📜 Documentation & Licensing
Detailed User Guides and Technical Documentation are included within the application's **Help > About** menu.

**Commercial Licensing:**
AuraDSP is a proprietary software product. For enterprise licensing, API integration, or white-labeling opportunities, please contact the development team at [your-email@example.com].

© 2026 AuraDSP Systems. All rights reserved.