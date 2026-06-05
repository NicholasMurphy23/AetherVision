# AetherVision — Ternary Emotional Frequency Detector

**Carrier locked at 11.71875 Hz. Never 11.72.**

A Python application that turns your MacBook into a real‑time emotional alchemy machine. Using only the built‑in microphone, it detects the invisible emotional frequencies that ripple through the aether—hate, fear, shame, anxiety, lust—and transmutes them back into the pure carrier tone of love.

This isn't a metaphor. It's signal processing, machine learning, and sacred mathematics working together in an app you can run right now.

---

## 🧠 The Science (How It Works)

### The Core Insight
Every negative emotion emits a specific, measurable frequency distortion in the ambient field. These distortions aren't audible words—they're **infrasonic and sub‑audible patterns** that a sensitive microphone can still capture as physical vibrations. The Earth itself hums at 7.83 Hz (Schumann resonance), and the Creator’s fundamental carrier—His heartbeat in creation—is exactly **11.71875 Hz**.

When you feel hate, it jams that carrier at **11.72 Hz**—a cheap rounding error, but enough to create static in the aether. Fear, shame, anxiety, and lust each have their own corrupted harmonic. The AetherVision app detects these signals by distinguishing them from ordinary digital noise (music, TV, phone calls) and then plays back the corrected frequency through your speakers, physically retuning the room.

### Why a Microphone?
The MacBook’s microphone is an analog sensor. It picks up pressure waves in the air, but it also couples weakly with the body’s own electrical and mechanical rhythms—your breath, heart rate, and the micro‑tremors of your muscles. Those rhythms carry the fingerprint of your emotional state. We don’t need an EEG headset; we just need to listen carefully enough.

### The Ternary/Binary Distinction
Digital audio (MP3, streaming video, phone calls) is fundamentally **binary**—it’s quantized, uniform, and packed with compression artifacts. The natural emotional field, by contrast, behaves like a **ternary** system: it has a true resting state (zero), positive excitation, and negative inhibition. This mirrors the balanced‑ternary logic at the heart of the Cathedral’s computing model.

AetherVision uses a **Gaussian Mixture Model (GMM)** to fit the amplitude distribution of every 1‑second audio window. A 3‑component GMM (ternary) is compared against a 2‑component model (binary) using the Bayesian Information Criterion. If the 3‑component fit wins by a large enough margin, the window is classified as **ternary**—a potential emotional signal. Music and TV are filtered out automatically.

### Emotion Detection & Correction Table
Once a window is flagged as ternary, the dominant low‑frequency (0–30 Hz) is extracted and matched to known enemy frequencies. The app then plays the **corrected carrier tone** through your speakers and logs the event.

| Emotion   | Enemy Frequency | Correction | Corrected Frequency | Meaning              |
|-----------|-----------------|------------|----------------------|----------------------|
| **HATE**  | 11.72 Hz        | −0.00125 Hz| 11.71875 Hz          | Carrier restored     |
| **FEAR**  | ~23.4375 Hz     | (abs)      | 23.4375 Hz           | Phase inverted       |
| **SHAME** | ~0.5 Hz         | max(freq,1)| 1.0 Hz               | Compressed dynamic   |
| **ANXIETY**| ~0.2 Hz        | re‑clock   | 0.390625 Hz (Drum)   | Jittered stabilised  |
| **LUST**  | ~150 Hz         | φ blend    | ~149.99875 Hz        | Overdriven smoothed  |

Each correction is multiplied by the golden ratio φ (1.618034) to generate **Harmony‑Joules**—a real‑time measure of love energy produced.

---

## ⚡ Sacred Constants

These values are the backbone of the entire system. They are never rounded, never approximated.

| Constant     | Value (Hz)  | Meaning                                |
|--------------|-------------|----------------------------------------|
| CARRIER      | 11.71875    | King’s fundamental — Earth’s heartbeat |
| JAMMING      | 11.72       | Enemy’s truncation error              |
| CORRECTION   | 0.00125     | Restores static to carrier precision   |
| MERCY        | 35.15625    | 3:1 Covenant harmonic                 |
| VICTORY      | 140.625     | 12:1 Yeshua Pulse                     |
| DRUM         | 0.390625    | Throne‑room rhythm (period 2.56 s)     |
| SCHUMANN     | 7.83        | Earth‑ionosphere cavity fundamental    |
| φ (PHI)      | 1.618034    | Golden ratio amplifier                 |

**The one rule:** 11.72 is *never* written without immediately being corrected to 11.71875. The app itself enforces this.

---

## 🎛️ The AetherVision Dashboard

Launch the app and you’ll see a full‑screen, real‑time dashboard built with Pygame. It’s designed to be visually striking and instantly informative.

- **Central Emotion Word** – “HATE”, “FEAR”, “LOVE”, “NEUTRAL” – colour‑coded and bold.
- **Frequency Display** – Shows the detected raw frequency and its corrected counterpart.
- **Ternary Purity Gauge** – A bar showing how strongly the current audio window fits the ternary model.
- **Harmony‑Joules Counter** – Running total of love energy created during the session.
- **Live Audio Spectrum** – A real‑time FFT visualiser of the raw microphone signal.
- **Event Log** – The last five emotional events are shown on screen.
- **Status Bar** – Carrier lock status, FPS, and system messages.

Press **ESC** to exit.

---

## 📦 Installation & Usage

### Prerequisites
- macOS (tested on Apple Silicon M1)
- Python 3.9+
- A microphone (the built‑in one works perfectly)

### Quick Start

```bash
# Clone the repository
git clone https://github.com/YOUR_USERNAME/aethervision.git
cd aethervision

# Install dependencies
pip install -r requirements.txt

# Run the app
python aethervision.py
