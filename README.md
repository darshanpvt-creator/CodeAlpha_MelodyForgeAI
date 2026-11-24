# MelodyForge AI
### Deep Learning-Based Music Generation with LSTM and ONNX

MelodyForge AI is an experimental music generation application that explores the use of deep learning for musical sequence prediction. It uses a Long Short-Term Memory (LSTM) neural network trained with PyTorch to generate musical note sequences, with ONNX Runtime Web enabling model inference directly in the browser.

The project demonstrates an end-to-end workflow covering model training, model conversion, browser-based inference, and MIDI generation.

## Live Application

**[Launch MelodyForge AI](https://melodyforge-ai.netlify.app)**

## Key Capabilities

- **LSTM-Based Sequence Generation:** Uses recurrent neural network architecture to predict successive musical notes.
- **Deep Learning Model Training:** Implements model training and experimentation using PyTorch.
- **ONNX Model Deployment:** Converts the trained model into ONNX format for browser-based inference.
- **Browser-Based Generation:** Runs model inference through ONNX Runtime Web.
- **MIDI File Export:** Converts generated note sequences into downloadable MIDI files.
- **Interactive Web Interface:** Provides a straightforward interface for generating musical outputs.

## Technical Architecture

| Component | Technology |
|---|---|
| Programming Language | Python |
| Model Architecture | Long Short-Term Memory (LSTM) |
| Deep Learning Framework | PyTorch |
| Model Interchange Format | ONNX |
| Browser Inference | ONNX Runtime Web |
| Frontend | HTML, CSS, JavaScript |
| Deployment Platform | Netlify |

## System Workflow

1. **Data Preparation** – Prepare MIDI patterns as input sequences for model training.
2. **Model Training** – Train the LSTM network using PyTorch.
3. **Model Export** – Convert the trained PyTorch model into ONNX format.
4. **Model Loading** – Load the ONNX model into the browser using ONNX Runtime Web.
5. **Sequence Prediction** – Generate musical notes through model inference.
6. **MIDI Generation** – Assemble the predicted notes into a downloadable MIDI file.

## Repository Structure

```text
CodeAlpha_MelodyForgeAI/
│
├── data/
│   └── training/              # MIDI training samples
│
├── generated/                 # Generated MIDI output
│
├── models/
│   ├── melody_lstm.pth        # Trained PyTorch model
│   └── melody_lstm.onnx       # Exported ONNX model
│
├── site/
│   ├── index.html             # Application interface
│   ├── script.js              # Browser inference and MIDI generation
│   ├── style.css              # Application styling
│   └── models/
│       └── melody_lstm.onnx
│
├── app.py                     # Python application module
├── train.py                   # Model training
├── export_model.py             # ONNX model export
├── requirements.txt            # Python dependencies
└── README.md
```

## Installation and Local Execution

### Prerequisites

- Python 3.10 or later
- pip
- A modern web browser

### 1. Clone the repository

```bash
git clone https://github.com/darshanpvt-creator/CodeAlpha_MelodyForgeAI.git
cd CodeAlpha_MelodyForgeAI
```

### 2. Install dependencies

```bash
pip install -r requirements.txt
```

### 3. Train the model

```bash
python train.py
```

### 4. Export the model

```bash
python export_model.py
```

### 5. Launch the web interface

```bash
cd site
python -m http.server 8000
```

Navigate to:

`http://localhost:8000`

## Dataset

The current implementation uses procedurally generated MIDI patterns as its training dataset. The project is an experimental implementation intended to demonstrate LSTM-based musical sequence learning and generation. The diversity and quality of generated melodies are therefore dependent on the training patterns and model configuration.

## Potential Enhancements

- Expand the dataset with diverse musical sequences.
- Improve sequence prediction and melody consistency.
- Introduce genre-based generation.
- Add controls for tempo, note range, and melody length.
- Evaluate model performance using musical evaluation metrics.

## Project Information

**Project:** MelodyForge AI  
**Domain:** Artificial Intelligence and Deep Learning  
**Internship:** CodeAlpha Artificial Intelligence Internship  
**Author:** Darshan G.

**GitHub Repository:**  
https://github.com/darshanpvt-creator/CodeAlpha_MelodyForgeAI

**Live Application:**  
https://melodyforge-ai.netlify.app

---

*An experimental implementation exploring the application of recurrent neural networks to automated musical sequence generation.*
