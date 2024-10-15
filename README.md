# Dysarthric Speech Recognition using Transformer

This project focuses on building a speech recognition model for dysarthric speakers using a transformer-based architecture. The model is initially trained on a general dataset (LJ Speech) and then fine-tuned using control speakers' data to adapt it for recognizing speech from dysarthric patients.

## Table of Contents
- [Introduction](#introduction)
- [Model Architecture](#model-architecture)
- [Dataset](#dataset)
- [Training Process](#training-process)
- [Results](#results)
- [Installation](#installation)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

## Introduction
Dysarthria is a speech disorder resulting from neurological damage, leading to difficulties in speech articulation. This project aims to develop a speech recognition system to assist patients with dysarthria by improving automatic speech-to-text conversion.

The model is based on transformer architectures, which have proven effective in various NLP and speech recognition tasks.

## Model Architecture
The model uses a transformer-based encoder-decoder architecture. Below is a visual representation of the architecture:

![Model Architecture](images/transformer.png)
*(Include a diagram of your model architecture here)*

## Dataset

### LJ Speech Dataset
The model was initially trained using the **LJ Speech Dataset**, which contains general speech samples. This dataset provides a good foundation for the model, enabling it to learn general speech patterns and characteristics.

### Control Speakers Dataset
After training on the LJ Speech dataset, the model was fine-tuned with **Control Speakers Data**. The control speakers are used as a bridge to help the model adjust from normal speech to dysarthric speech, preparing it for the final stage of training with dysarthric patients.

### Dysarthric Speech Data
The final training stage focuses on speech data collected from dysarthric patients. This helps the model adapt and specialize in recognizing speech patterns commonly associated with dysarthria.

## Training Process
The training process consists of two major stages:

1. **Initial Training with LJ Speech**:
   - The model was first trained on the LJ Speech dataset to learn general speech patterns.
   - This dataset helps the model develop a broad understanding of speech features, which is later useful for adaptation.

2. **Fine-tuning with Control Speakers**:
   - After the initial training, the pre-trained model was loaded, and further training was conducted using the control speakers’ dataset.
   - This allows the model to adapt to the more specialized data, bridging the gap between general and dysarthric speech.

3. **Training with Dysarthric Speech** (Final Stage):
   - The model was then fine-tuned with dysarthric patients' speech data to specialize in recognizing the specific speech difficulties faced by these patients.

## Results
The model's performance has improved over time by gradually adapting from general speech to more complex dysarthric speech patterns. The final model shows significant improvements in recognizing dysarthric speech compared to traditional methods.

## Installation
To install and run the project, follow these steps:

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/dysarthric-speech-recognition.git
