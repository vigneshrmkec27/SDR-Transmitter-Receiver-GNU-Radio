
---

# 📡 AM Transmitter & Receiver using SDR and GNU Radio Companion

This project demonstrates the **Amplitude Modulation (AM) transmission and reception** process using **Software Defined Radio (SDR)** and **GNU Radio Companion (GRC)**.
It helps understand the fundamentals of analog communication by implementing AM signal generation, modulation, transmission, and demodulation in a software environment.

---

## 🧠 Project Overview

The project simulates an **AM Transmitter and Receiver** system using GNU Radio blocks.
It can transmit an audio signal (such as a .wav file or microphone input) and receive it back using an SDR or loopback configuration.

---

## ⚙️ Features

* 🎧 **Audio Input & Output** (Microphone or Audio File)
* 🧩 **AM Modulation and Demodulation**
* ⚡ **Adjustable Carrier Frequency and Gain**
* 🔁 **Real-Time Transmission & Reception**
* 💻 **Can Work Without SDR Hardware (Simulation Mode)**

---

## 🧩 System Requirements

| Component             | Description                          |
| --------------------- | ------------------------------------ |
| **Software**          | GNU Radio Companion (v3.8 or higher) |
| **Optional Hardware** | RTL-SDR, HackRF, or USRP             |
| **Operating System**  | Linux / Windows / macOS              |
| **Dependencies**      | Python 3.x (included with GNU Radio) |

---

## 🚀 How to Run the Project

### 🔧 Step 1: Install GNU Radio

```bash
sudo apt update
sudo apt install gnuradio
```

### 📂 Step 2: Clone this Repository

```bash
git clone https://github.com/<your-username>/am-transmitter-receiver.git
cd am-transmitter-receiver
```

### 📡 Step 3: Connect SDR Device (Optional)

If you have an SDR such as **RTL-SDR**, **HackRF**, or **USRP**, connect it and test:

```bash
rtl_test
```

### 🧠 Step 4: Open Flowgraphs

Open **GNU Radio Companion**:

```bash
gnuradio-companion
```

Then open:

* `am_transmitter.grc`
* `am_receiver.grc`

---

## ▶️ Execution Steps

1. **Run the Transmitter flowgraph** – generates and transmits the AM signal.
2. **Run the Receiver flowgraph** – receives and demodulates the AM signal.
3. Output can be played through speakers or visualized using a Scope Sink.

---

## 🧱 Block Diagram Overview

### **Transmitter Flowgraph**

```
Audio Source → Multiply (Carrier Signal) → Throttle → SDR Sink / Audio Sink
```

### **Receiver Flowgraph**

```
SDR Source / File Source → Envelope Detector → Audio Sink
```

---

## 🎥 Demo & Results

Below are sample visual results you can showcase in your README once you run your project 👇

### 🖼️ **1. Transmitted Signal (Time Domain)**

![Transmitter Waveform](resources/transmitter_waveform.png)

### 🌈 **2. Spectrum of AM Signal**

![Spectrum of AM Signal](resources/am_spectrum.png)

### 🎧 **3. Demodulated Audio Output**

![Demodulated Audio](resources/demodulated_audio.png)

> You can capture these plots using the **QT GUI Time Sink** and **QT GUI Frequency Sink** blocks in GNU Radio.

---

## 📘 Learning Outcomes

By completing this project, you will learn:

* ✅ The principle of **Amplitude Modulation (AM)**
* ✅ How to **design flowgraphs** in GNU Radio
* ✅ Understanding of **SDR signal processing chain**
* ✅ Hands-on skills in **modulation, demodulation, and real-time signal flow**

---

## 📁 Project Structure

```
📦 am-transmitter-receiver/
├── am_transmitter.grc
├── am_receiver.grc
├── README.md
└── resources/
    ├── sample_audio.wav
    ├── transmitter_waveform.png
    ├── am_spectrum.png
    └── demodulated_audio.png
```

---

## 🧰 References

* [GNU Radio Documentation](https://wiki.gnuradio.org/index.php/Main_Page)
* [RTL-SDR Quick Start Guide](https://www.rtl-sdr.com/rtl-sdr-quick-start-guide/)
* [SDR Basics: Analog Modulation](https://wiki.gnuradio.org/index.php/Category:Analog_Modulation)
* [HackRF One Documentation](https://greatscottgadgets.com/hackrf/)

---

## 🧑‍💻 Author

* **Vignesh G**
* **Advanced Communication Technology**
* 📍 **R.M.K Engineering College**

💬 *“Exploring the world of wireless communication through SDR.”*

If you found this helpful, ⭐ **star this repository** to support future projects!

---

## 📜 License

This project is licensed under the **MIT License** – you are free to use and modify it.

---

