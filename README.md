# 🎧 AM Transmitter and Receiver using SDR and GNU Radio

This project demonstrates **Amplitude Modulation (AM) Transmission and Reception** using **Software Defined Radio (SDR)** and **GNU Radio Companion (GRC)**.  
It includes flowgraphs that show how an analog signal can be modulated, transmitted, and received — all in software, without needing complex RF hardware setups.

---

## 📜 Project Overview

**Objective:**  
To design and implement an **AM Transmitter** and **Receiver** using **GNU Radio** and an SDR platform, visualizing the modulation and demodulation process in real-time.

**Key Concepts Covered:**
- Analog Modulation (Amplitude Modulation)
- Software Defined Radio fundamentals
- Flowgraph design in GNU Radio Companion
- Real-time signal visualization (Scope, FFT, Waterfall)

---

## ⚙️ Technologies & Tools Used

| Component | Description |
|------------|--------------|
| **GNU Radio** | Open-source toolkit for signal processing |
| **GNU Radio Companion (GRC)** | GUI tool for building signal flowgraphs |
| **SDR Hardware (Optional)** | RTL-SDR / HackRF / USRP / Any supported SDR device |
| **Python** | Backend flow execution language for GNU Radio |
| **Ubuntu / Windows Subsystem for Linux** | Recommended OS environment |

---

## 🧩 Project Structure

📁 AM-Trans-and-Rec-SDR
│
├── 📂 transmitter
│ └── am_tx.grc # Flowgraph for AM Transmission
│
├── 📂 receiver
│ └── am_rx.grc # Flowgraph for AM Reception
│
├── 📄 README.md # Documentation (this file)
└── 📄 requirements.txt # (Optional) Dependencies for setup


---

## 🚀 How to Run the Project

### 🔧 Step 1: Install GNU Radio

```bash
sudo apt update
sudo apt install gnuradio

📡 Step 2: Connect SDR Device (Optional)

If you have an SDR (like RTL-SDR, HackRF, or USRP), plug it in and check:

rtl_test

🧠 Step 3: Open Flowgraphs

Open GNU Radio Companion:

gnuradio-companion


Then:

Load am_tx.grc for transmission

Load am_rx.grc for reception

▶️ Step 4: Run the Flowgraphs

Execute the transmitter flowgraph first

Then run the receiver flowgraph

Observe signals using:

Time Sink

FFT Sink

Waterfall Sink

📈 Expected Output

Transmitter: Converts baseband audio signal into an AM-modulated RF signal.

Receiver: Demodulates AM signal and retrieves the original audio.

Visualizations:

FFT plot showing carrier + sidebands

Time-domain waveform of modulated and demodulated signal

📚 Resources & References
Type	Resource
🎓 GNU Radio Docs	https://wiki.gnuradio.org

📘 SDR Concepts	https://www.rtl-sdr.com

🎥 Tutorial Video	HackRF + GNU Radio AM Tutorial (YouTube)

📗 Book	Software Defined Radio using MATLAB & Simulink and the RTL-SDR – Robert W. Stewart
🧩 GitHub Example	https://github.com/gnuradio/gnuradio
🧠 Learning Outcomes

By completing this project, you will:

Understand Amplitude Modulation principles

Learn to design signal flowgraphs in GNU Radio

Visualize modulation, transmission, and demodulation in real-time

Experience hands-on SDR-based communication systems

💡 Future Enhancements

Add Frequency Modulation (FM) or SSB mode

Implement Noise filtering

Integrate USRP hardware for long-range communication

Add a GUI-based control panel using PyQt or Tkinter

👨‍💻 Author

Vignesh G
Advanced Communication Technology
📫 Feel free to connect or star this repo if you find it helpful!

🔗 LinkedIn
 | GitHub

🪪 License

This project is licensed under the MIT License — feel free to use and modify for educational purposes.

🌟 Support & Contributions

Contributions, issues, and feature requests are welcome!
Feel free to fork this repository and submit a pull request.

If you found this project useful, please ⭐ it on GitHub!


---

Would you like me to:
- 🖼️ Add **diagrams (block diagram of AM TX/RX)** inside the README?  
- or 🧑‍💻 Add **badges** (like build status, tech stack icons, etc.) to make it look more professional?

I can generate the next version with visuals and badges for you.

