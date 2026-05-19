# vigilant-octo-spoon

# Multimodal Crime Scene Video Summarization using Audio-Visual Fusion

Example Summarized Videos: https://canva.link/8zqvgo44qoobdnx
<img width="714" height="534" alt="image" src="https://github.com/user-attachments/assets/359c89eb-7f11-48c7-8a4d-51f7e9872191" />


## Overview
This project was developed as part of my MSc Artificial Intelligence coursework and focuses on **automated crime scene video summarization** using a **multimodal fusion approach** combining **audio** and **visual** information.

Traditional surveillance review relies heavily on manual inspection of lengthy video footage, which is time-consuming and inefficient. This project addresses that problem by automatically identifying and extracting important video segments using:

- **Audio event detection** (e.g., gunshots, sirens, screams, alarms)
- **Visual object detection and tracking** (e.g., people, vehicles, hazardous scenes)

The result is a concise summary video that preserves critical events while significantly reducing review time.

---

## Problem Statement
Security personnel often need to manually review hours of surveillance footage to identify important incidents.

This project aims to:
- reduce manual review time,
- improve surveillance efficiency,
- and support faster incident response through automated summarization.

---

## Project Objectives
The system was designed to:
- detect high-risk audio events,
- identify visually important objects and scenes,
- fuse audio and visual signals,
- and generate a summarized version of the original surveillance footage.

---

Technologies Used
- Python
- Google Colab
- YOLOv8
- TensorFlow
- OpenCV
- Librosa
- Matplotlib

Dataset

Audio data was derived from AudioSet.

Selected subsets:

- Balanced Training Set
- Evaluation Set

These provided labelled real-world audio events for benchmarking.

## System Architecture

Pipeline:

```text
Input Video
   ↓
Audio Extraction
   ↓
Audio Analysis (YAMNet)
   ↓
Visual Analysis (YOLOv8)
   ↓
Multimodal Fusion
   ↓
Importance Scoring
   ↓
Video Summary Generation
```

Future Improvements

Potential future work includes:

- testing on larger real-world CCTV datasets
- transformer-based multimodal fusion
- real-time streaming support
