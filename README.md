# Text Summarizer

An AI-powered text summarization application built using Python, Hugging Face and Gradio. The application takes user-provided text and generates a concise summary using a pretrained DistilBART model through a Hugging Face Inference Endpoint.

## Features

- Summarizes user-provided text using a pretrained NLP model
- Uses Hugging Face Inference API for model inference
- Simple and interactive web interface using Gradio
- Supports abstractive text summarization
- Provides a shareable Gradio interface

## Tech Stack

- **Python**
- **Hugging Face**
- **DistilBART**
- **Gradio**
- **API**

## How It Works

The application follows this flow:

User Input
→ Gradio Interface
→ `summarize()` function
→ `get_completion()`
→ Hugging Face Inference Endpoint
→ DistilBART Model
→ Generated Summary
→ Gradio Output

The application sends the input text to a Hugging Face Inference Endpoint using an HTTP POST request. The endpoint processes the text using the pretrained `shleifer/distilbart-cnn-12-6` model and returns the generated summary.

## Project Structure

```text
Text-Summarizer/
│
├── text summarizer.ipynb
└── README.md
