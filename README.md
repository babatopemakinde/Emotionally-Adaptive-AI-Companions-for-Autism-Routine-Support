# Multimodal Emotion AI for ASD Support (Post-Publication Engineering)


A production-grade emotion recognition system designed to support autistic adolescents by detecting emotional states in real time through facial expressions and vocal cues.

Architecture: EfficientNet-B0 (vision) + MFCC-CNN (audio) with attention-gated fusion, trained on RAVDESS and the Autistic Children Emotions dataset across six emotion classes: anger, fear, joy, sadness, surprise, and neutral.

Explainability: Guided Grad-CAM (4 artefacts per inference) for vision and SHAP DeepExplainer for audio, enabling transparent, interpretable predictions suitable for clinical and educational settings.

Outputs: Fused emotion probabilities, adaptive behavioural intervention plans, visual schedule cards, and TTS audio guidance — all contextualised by environment, routine, and time of day.

Use case: Assistive AI for therapists, educators, and caregivers working with autistic adolescents in school, home, and therapy settings.




**Emotionally-Adaptive-AI-Companions-for-Autism-Routine-Support**


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
