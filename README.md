# Grammar-Scoring-Engine
A Grammar Scoring Engine for spoken data samples, built using Whisper for ASR (Automatic Speech Recognition) and LanguageTool for grammar evaluation. This project is designed to transcribe spoken voice samples into text and score the grammar of the transcriptions, with an enhanced penalty system for more accurate scoring.

## Project Overview
This repository contains a **Grammar Scoring Engine** that processes spoken voice samples, transcribes them into text using **Whisper**, and evaluates the grammar of the transcriptions with **LanguageTool**. The engine introduces a stricter scoring system, applying heavier penalties for grammatical errors, which generates a wider range of scores. 

The dataset used for this project is proprietary and provided by SHL. The engine is run in a **Google Colab** environment for easy execution.

## Features
- **Speech-to-Text Conversion**: Uses **Whisper** to convert audio samples into text.
- **Grammar Evaluation**: Utilizes **LanguageTool** to assess and score the grammar of the transcriptions.
- **Stricter Scoring System**: Applies a more rigorous penalty system for errors to produce a broader range of grammar scores.
- **Custom Dataset**: Works with a proprietary dataset from **SHL**, including both training and testing audio files.

## Dataset
The dataset consists of **audio files** and their corresponding transcriptions:

- **Audio (Train)**: `/content/shl/dataset/audios_train`
- **Audio (Test)**: `/content/shl/dataset/audios_test`
- **CSV Files**: `/content/shl/dataset/train.csv` and `/content/shl/dataset/test.csv`

### Columns in the CSV Files:
- `audio_filename`: Name of the audio file.
- `transcription`: The ground-truth transcription of the spoken audio (for training).

## Requirements
- Python 3.7+
- Google Colab (or local Jupyter Notebook)
- Whisper
- LanguageTool
- Pandas, NumPy, and other Python libraries

## Installation
1. Clone the repository:

   ```bash
   git clone https://github.com/yourusername/grammar-scoring-engine.git
   cd grammar-scoring-engine
