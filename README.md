# SONARIX AI

### AI-Assisted Speech Enhancement for High-Noise Environments

SONARIX AI is an AI-assisted speech enhancement system that is made to make human voice clearer in places that're very noisy and have a lot of interference.

The system uses **Digital Signal Processing (DSP)**. *Deep Learning** together to get rid of unwanted sounds in the background while making the voice better and easier to understand.

 🎯 Problem

In places that're very noisy such as near engines, helicopters, machines and outside work areas regular ways to reduce noise can make the background quieter but they can also make the voice sound worse or not as clear.

SONARIX AI is made to fix this problem by using AI to figure out what is speech and combining it with DSP to process the signal.

 💡 Proposed Solution

SONARIX AI takes audio and goes through a mix of steps:

**Noisy Audio → Preprocessing → STFT → AI Mask Estimation → DSP Fusion → Speech Reconstruction → Enhanced Speech**

The AI model finds which parts of the audio probably have speech that is useful and the DSP processing helps to put the signal back together and make it better.

✨ Key Features
* AI-based speech mask estimation
* DSP-assisted noise suppression
* Speech preservation
* loudness enhancement
* STFT-based signal processing
* Configurable noise conditions
* MATLAB-based simulation and evaluation
* Designed for edge deployment

🧠 Technical Approach
 1. Audio Acquisition
Recorded speech is put together with kinds of background noise at specific levels of signal and noise.
2. Preprocessing
The audio is made to have the loudness and split into small parts for time and frequency analysis.
3. STFT Analysis
The Short-Time Fourier Transform (STFT) takes the audio. Changes it from time-based to time and frequency-based.
4. AI Mask Estimation
A neural network looks at the frequency-based audio and guesses which partsre likely to have speech.
5 Ai Fusion

The guess from the network is used with DSP to make sure the bad parts are removed but the important parts of the speech are kept.

### 6. Speech Reconstruction

The better sound is changed back into time-based form using an inverse STFT.

### 7. Output Enhancement

A final step makes the speech more clear. Gives the final improved audio.

---

## 🛠️ Technologies Used

* **MATLAB**

* **Deep Learning Toolbox**

* Digital Signal Processing

* Short-Time Fourier Transform (STFT)

* Neural Networks

* Audio Signal Processing

📂 Project Structure

SONARIX_AI/

│

├── src/

│   ├── generated_noisy_audio.m

│   ├── sonarix_ai_training.m

│   ├── sonarix_ai_inference.m

│   └── localSTFT.m

│

├── dataset/

│   ├──

│   ├── engine/

│   ├── helicopter/

│   ├── wind/

│   └── impulse/

│

├── generated/

│   ├── SNR_0dB/

│   ├── SNR_5dB/

│   ├── SNR_10dB/

│   ├── SNR_15dB/

│   └── SNR_20dB/

│

├── models/

├── results/

├── docs/

│

├── README.md

└──.gitignore

> Big audio data and trained models might not be in the public version to keep the size small.

---

## 📊 Current Experimental Results

The MATLAB simulation currently uses:

| Parameter                 Value |

| ------------------ | ----------: |

| Sampling Frequency |    44.1 kHz |

| Frame Length              32 ms |

| Hop Length         | 706 samples |

| FFT Size           |        2048 |

| Training Frames    |      20,000 |

| Validation Frames  |       5,000 |

| Total Frames       |      25,000 |

| Training Epochs    |          15 |

### Validation Performance

| Metric        |   Result |

| ------------- | -------: |

| RMSE          | 0.245846 |

| MAE            0.163059 |

| R²            | 0.664232 |

| Correlation   | 0.815329 |

| Mask Accuracy |   52.57% |

These results are for the **current experimental MATLAB model** and are meant to be a start for the next steps.

---

## ▶️ How to Run

### Requirements

* MATLAB

* Deep Learning Toolbox

* Audio Processing capabilities

### Step 1. Clone the repository

```bash

git clone https://github.com/harshacodes0/SONARIX_AI.git

```

### Step 2. Open the project in MATLAB

Go to the project folder. Start MATLAB.

### Step 3. Generate audio

Run:

```matlab

generated_noisy_audio

```

### Step 4. Train the AI model

Run:

```matlab

sonarix_ai_training

```

### Step 5. Run inference

Run:

```matlab

sonarix_ai_inference

```

The improved audio will be in the results/output folder.

---

## 🚀 Future Development

* time audio processing

* Raspberry Pi 5 deployment

* Microphone-array integration

* Lightweight edge AI inference

* speech-preservation performance

* Adaptive noise suppression

* Real-time voice amplification

* Hardware prototype development

---

## 🎯 Target Application

SONARIX AI is being made for places where its hard to hear voices because of a lot of background noise. These places include:

* Defence and field operations

* environments

* Aviation environments

* Areas with a lot of machines

* Emergency communication systems

---

## 📌 Project Status
Current Stage: MATLAB software simulation and AI model development

Future Stage: Edge implementation and hardware prototype


## 👩‍💻 Author

**Harsha**

B.Tech Electronics and Communication Engineering

GitHub: `@harshacodes0`


## 📄 License

This project is, for research and prototype-development use.
