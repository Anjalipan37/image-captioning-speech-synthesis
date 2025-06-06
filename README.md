# Automated Image Captioning with Speech Synthesis 

This project combines the power of deep learning and speech synthesis to create an assistive tool that can **generate image captions** and **speak them aloud**. It’s designed especially for improving accessibility for visually impaired users by enabling machines to describe images in natural language and convert that description to audio in real time.

---

##  Project Highlights

-  Extracts visual features using a pre-trained **DenseNet201** CNN.
-  Generates meaningful image captions with an **LSTM-based RNN**.
-  Converts captions into **speech output** using `gTTS` or `pyttsx3`.
-  Evaluated using **BLEU** and **METEOR** scores for quality assurance.

---

##  Motivation

Interpreting visual content comes naturally to humans, but it's a complex task for machines. Our goal was to bridge this gap and make visual data more accessible, especially for people with visual impairments. By combining image recognition, language generation, and text-to-speech, we created a system that can "see," "describe," and "speak."

---

##  Tech Stack

- **Language**: Python
- **Deep Learning**: TensorFlow / Keras
- **Image Processing**: DenseNet201 (CNN)
- **Sequence Modeling**: LSTM (RNN)
- **Text-to-Speech**: gTTS (online) / pyttsx3 (offline)
- **Data Handling & Visualization**: NumPy, Pandas, Matplotlib

---

##  Dataset Used

We used the **Flickr8k** dataset, which includes:
- 8,000 real-world images
- 5 human-written captions per image (40,000 total captions)
- Diverse image subjects: people, animals, scenes, and objects

---

##  Model Pipeline

1. **Image Input**: Upload or capture an image.
2. **Feature Extraction**: DenseNet201 converts image to feature vector.
3. **Caption Generation**: LSTM generates a descriptive sentence.
4. **Text-to-Speech**: Caption is converted to audio using TTS.
5. **Output**: User receives both text and spoken description.

---

##  Results

- **BLEU Score**: Achieved a score of ~0.6, indicating strong caption relevance.
- **METEOR Score**: Used to verify semantic accuracy and grammar.
- **Real-Time Output**: Captions generated and spoken within 2–5 seconds.

---

##  Applications

-  **Assistive Tech** for visually impaired users
-  Autonomous vehicles and robotics
-  E-commerce: Visual search and product tagging
-  Social media: Auto-captioning images
-  Smart home monitoring
-  Healthcare: Medical image explanation

---

##  Limitations

- Requires quality training data to perform well
- May struggle with abstract or highly complex scenes
- Real-time performance depends on system resources (GPU recommended)
- Language limited to English (can be extended)

---

##  Future Scope

- Integrate **Transformer models** for improved accuracy
- Support **multi-language captioning and TTS**
- Add **object detection** for more detailed descriptions
- Optimize for **mobile and embedded systems**
- Enable **creative captioning** for social platforms

---

##  How to Run

1. Clone the repo:
   ```bash
   git clone https://github.com/your-username/image-captioning-speech-synthesis.git
