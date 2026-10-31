# SHORTWAVE-Simulation-
A Python-based shortwave SDR simulator featuring adjustable frequency tuning, USB/LSB demodulation simulation, real-time spectrum analysis, waterfall visualisation, and synthetic audio output. Designed as a foundation for future software-defined radio development. (Fully coded by ChatGpt)

# SHORTWAVE
### Software Defined Radio Simulator

SHORTWAVE is a Python-based software-defined radio (SDR) simulation designed to replicate the experience of operating a shortwave radio receiver.

The application provides an interactive interface for frequency tuning, simulated USB and LSB reception, real-time spectrum analysis, waterfall visualisation and synthetic audio output.

**Important:** SHORTWAVE currently operates entirely through simulated signals. It does not receive real radio transmissions or connect to physical SDR hardware.

---

## Features

- **Frequency Tuning:** Adjustable frequencies from 100 kHz to 30 MHz.
- **USB / LSB Modes:** Switch between Upper Sideband and Lower Sideband simulation.
- **Spectrum Analyser:** Real-time visualisation of simulated signal strength.
- **Waterfall Display:** Visualises frequency activity over time.
- **Audio Output:** Generates synthetic radio-like audio.
- **Tuning Steps:** Adjustable tuning increments from 10 Hz to 5 kHz.
- **Minimal Interface:** Dark-themed interface built using PyQt6.

---

## Technologies

| Technology | Purpose |
|---|---|
| Python | Main programming language |
| PyQt6 | Graphical user interface |
| NumPy | Numerical and signal processing |
| SciPy | Scientific computing and signal processing |
| PyQtGraph | Spectrum and waterfall visualisation |
| SoundDevice | Audio output |

---

## Requirements

- Windows 10 or Windows 11
- Python 3.12 or 3.13 recommended
- Internet connection for initial installation
- Audio output device for simulated audio

Python downloads:

https://www.python.org/downloads/

---

## Installation

### 1. Clone the repository

Open PowerShell or the VS Code terminal.

```powershell
git clone https://github.com/YOUR-USERNAME/SHORTWAVE.git
```

Replace `YOUR-USERNAME` with your GitHub username.

Enter the project directory:

```powershell
cd SHORTWAVE
```

Alternatively, download the repository as a ZIP file from GitHub and extract it.

### 2. Create a virtual environment

```powershell
py -m venv .venv
```

### 3. Activate the environment

For PowerShell:

```powershell
.\.venv\Scripts\Activate.ps1
```

If PowerShell blocks activation, you can skip activation and use the full Python path in the following commands.

### 4. Install dependencies

```powershell
python -m pip install --upgrade pip
```

```powershell
python -m pip install numpy PyQt6 pyqtgraph sounddevice
```

### 5. Run the application

```powershell
python shortwave_simulator.py
```

The SHORTWAVE application should now launch.

---

## Running Without Activating the Environment

You can also run everything directly through the virtual environment:

Install dependencies:

```powershell
.\.venv\Scripts\python.exe -m pip install numpy PyQt6 pyqtgraph sounddevice
```

Launch:

```powershell
.\.venv\Scripts\python.exe .\shortwave_simulator.py
```

---

## How to Use

**Frequency Tuning**

Enter a frequency using the frequency control. The application supports frequencies between 100 kHz and 30 MHz.

**USB / LSB**

Select either:
- USB — Upper Sideband
- LSB — Lower Sideband

**Tuning Step**

Choose the frequency increment you want to use when tuning.

**Spectrum**

The spectrum analyser displays simulated signal activity around the selected frequency.

**Waterfall**

The waterfall display shows signal activity over time, allowing you to observe changes in the simulated radio environment.

**Audio**

Press START AUDIO to hear synthetic radio-like signals. Press STOP AUDIO to stop playback.

---

## Project Status

**Current version: 0.1.0 — Simulation**

SHORTWAVE is currently a software simulation and development project.

Planned future improvements:

- Real SDR hardware integration.
- RTL-SDR compatibility.
- Real-time RF spectrum analysis.
- Actual USB and LSB demodulation.
- Improved signal filtering.
- Additional modulation modes.
- Signal recording and playback.

---

## Disclaimer

This application generates simulated radio signals for educational and development purposes.

It does not currently capture, decode or receive actual radio-frequency transmissions.

---

## License

This project is released under the MIT License.

See the LICENSE file for details.

---

## Author

Developed as an independent Python and software-defined radio learning project.
