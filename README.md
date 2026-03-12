# Emotionally-Adaptive-AI-Companions-for-Autism-Routine-Support
Research on emotionally adaptive AI companions designed to assist autistic adolescents with routine management through personalised and emotion-aware interaction.

Emotionally Adaptive AI Companion for Autistic Adolescents

This project presents a prototype for an Emotionally Adaptive AI Companion designed to support autistic adolescents in managing daily routines, emotional regulation, and social transitions. Unlike static support tools, this system uses real-time multimodal emotion recognition to provide personalized, context-aware interventions.

Key Features
Multimodal Emotion Recognition: Uses facial expressions and simulated voice tones to detect emotional states like stress or anxiety.
Context-Aware Engine: Integrates situational data—such as time of day, location, and specific tasks—to tailor support.
Human-in-the-Loop Feedback: Allows caregivers to log the effectiveness of interventions, creating a continuous learning loop to refine future support.
Interactive Interface: A Gradio-based UI that facilitates real-time interaction and immediate feedback.

Technical Architecture
1. Sensing Layer (Data Input)
The system processes two primary streams: Visual: Facial expressions captured via image data.
Auditory: Simulated voice emotion features synthetically generated from facial embeddings.

2. Emotion Recognition Models
The project utilizes Transfer Learning across three Convolutional Neural Network (CNN) architectures:
ResNet-18
EfficientNet-B0
MobileNetV2

3. Fusion and Inference
Late-Fusion: Combines visual (70% weight) and auditory (30% weight) distributions to determine the final emotional state.
Decision Engine: A rule-based engine selects interventions (e.g., calm music, reassurance) based on the detected emotion and current context.
