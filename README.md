# 🎻 QaraamiGen AI: Oud Transcription Engine
Preserving Somali Musical Heritage through Deep Learning

QaraamiGen AI is a specialized Automatic Music Transcription (AMT) system trained to recognize the unique frequencies and rhythms of the Somali Pentatonic Scale. By analyzing traditional Oud recordings, the model converts raw audio into ABC Notation for digital preservation and sheet music generation.

🧠 Training Highlights
We trained a custom Convolutional Neural Network (CNN) over 20 epochs, achieving a significant improvement in accuracy:

Starting Loss: 2.7111 (Epoch 1)

Final Loss: 0.2913 (Epoch 20)

Accuracy: The model successfully mapped audio features to 15 distinct musical classes (notes) within the Qaraami scale.

🛠 Tech Stack
Dataset: 50 curated clips of traditional Oud, labeled with fundamental frequencies (Hz) and musical notes.

Architecture: PyTorch-based CNN (QaraamiTranscriptor) designed for spectral feature extraction.

Audio Processing: Librosa for Mel-Spectrogram generation and onset detection.

Backend: FastAPI for serving real-time transcriptions to a Next.js frontend.

📂 Project Structure
/dataset: Contains metadata.jsonl and the audio source references.

/backend: FastAPI logic and the trained weights file qaraami_model_v1.pth.

/frontend: Next.js source code including the OudRecorder and ABCJS integration.

🚀 Future Vision
The goal of this project is to create a digital bridge between the cassette-tape era of Somali music and the modern era of algorithmic preservation.