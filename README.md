# 🎵 Reson8

**Reson8** is an interactive web-based Pulse Sequence Laboratory that transforms musical melodies into MRI-compatible gradient waveforms. 
Using Google's Gemini AI, it allows users to "compose" for the scanner, visualizing how auditory frequencies translate into magnetic field oscillations.

[Live Demo](https://benzoch.github.io/Reson8/)

---

## 🚀 The Concept

MRI scanners make noise because of the **Lorentz forces** acting on gradient coils. 
By pulsing these gradients at specific frequencies, the scanner effectively becomes a giant, multi-million dollar musical instrument. 

**Reson8** bridge the gap between medical imaging and digital synthesis:
1. **AI Composition:** Use Gemini to turn text prompts into musical notation.
2. **Gradient Mapping:** Automatically calculate amplitudes based on hardware constraints ($G_{max}$ and $S_{max}$).
3. **Visual Lab:** View the real-time X/Y gradient waveforms required to "play" that note.

---

## 🛠 Features

- **🤖 AI-Powered:** Describe a mood (e.g., "A spooky space walk") and let the AI generate the sequence.
- **📉 Real-time Waveform Visualization:** See the 10μs sampled gradient pulses.
- **🔊 Audio Preview:** Hear the melody before you send it to the "scanner."
- **⚙️ Hardware Constraints:** Adjustable Gradient Strength (mT/m) and Slew Rate (T/m/s) to simulate different scanner architectures.

---

## 📖 How to Use

1. **Enter API Key:** Paste your Gemini API key in the top right (this stays in your browser's memory and is never stored).
2. **Compose:** Use the **AI Composer** or manually type notes in `NOTE:DURATION` format (e.g., `C4:250 E4:250`).
3. **Simulate:** Adjust the sliders to see how hardware limits affect the waveform amplitude to prevent hardware damage (simulated).
4. **Play:** Hit **Preview Sound** to hear the resonance.

---

## 🛠 Tech Stack

- **React 18** - UI Logic
- **Tailwind CSS** - Modern Styling
- **Babel Standalone** - In-browser JSX Transpilation
- **Gemini API** - Generative Music Composition
- **Web Audio API** - Note Synthesis

---

## ⚠️ Disclaimer

*This is a simulation tool for educational and creative purposes. 
While it uses real MRI physics principles (like the relationship between frequency, amplitude, and slew rate), the generated sequences should not be used on a real MRI scanner without professional pulse sequence programming and safety validation.*
