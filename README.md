# Hindi-GPT

## Overview

This repository contains the steps to run **Hindi-GPT**, a powerful tool for converting speech into text and providing responses in Hindi.

## Getting Started


Follow these steps to get started with the **Hindi-GPT:

1. Download the Whisper Hugging Face model:
   - [Whisper Model Endpoint](https://huggingface.co/openai/whisper-medium)

2. Download the Llama 7B 5-bit Quantization module (llama-2-7b-chat.Q5_K_S.gguf):
   - [Llama 7B 5-bit Quantization Module](https://huggingface.co/TheBloke/Llama-2-7b-Chat-GGUF/tree/main)

3. Download the Text(English) to Text(Hindi) model:
   - [mbart-large-50-one-to-many-mmt](https://huggingface.co/facebook/mbart-large-50-one-to-many-mmt)

   **Note:** Please remember to update the `config.json` file after installation and upload llama in models/ dir.

## Installation
Code
```bash
   https://github.com/rishabbjain/Hindi-Gpt.git
   cd Hindi-Gpt

```
Requirements
```bash
   Python 3.8.18
   pip install -r requirements.txt
```
## Data

You can provide input audio data in either WAV or MP3 formats, with a required sampling rate of 16KHz.

To use your own audio data, follow these steps:

- Ensure the audio file is in either WAV or MP3 format.
- Make sure the audio file has a sampling rate of 16KHz.

Next, update the `config.json` file with the path to your input audio file:

```json
{
  "audio-file": "../audio-samples/<your-audio.wav>"
}

