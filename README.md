# LipNet - Deep Learning Based Lip Reading System

![Demo](app/animation.gif)

This project implements a **Lip Reading system** using **Deep Learning** techniques like CNNs and Connectionist Temporal Classification (CTC). It converts silent lip movements from videos into readable text.

---

## Features
- Lip reading from video without audio
- Deep learning model with CNN + RNN + CTC loss
- Pre-trained model checkpoints
- Streamlit app for real-time testing
- Visual feedback using saliency maps

---

## How It Works

1. **Video Input**: A speaker’s face is recorded while speaking.
2. **Preprocessing**: Extracts lip region and normalizes frames.
3. **Feature Extraction**: CNN layers extract spatial features.
4. **Temporal Modeling**: RNN (usually GRU/LSTM) understands motion.
5. **Decoding**: CTC loss enables sequence decoding without alignment.
6. **Output**: Predicted text from silent video input.

---

## Dataset Used
- **GRID Corpus**  
  34 speakers × 1000 sentences each  
  ~34,000 video samples  
  Format: short structured sentences with fixed patterns

---

## Run the App

### 1. Install Dependencies

```bash
pip install -r requirements.txt

```
### 2. Launch the Streamlit App

```bash
streamlit run app/streamlitapp.py
