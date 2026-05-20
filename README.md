
# Understanding Temporal Action Localisation using ActionFormer

A research oriented project exploring transformer-based temporal action localisation using ActionFormer on the THUMOS14 dataset under memory constrained settings.

---

# Overview

This project investigates the behaviour and evaluation of transformer based temporal action localisation models using the ActionFormer architecture.

Unlike traditional image classification, temporal action localisation requires a model to:
- identify actions in untrimmed videos
- predict temporal start and end boundaries
- classify action categories
- handle overlapping and background segments

The project focuses on:
- understanding ActionFormer
- analysing localisation behaviour
- evaluating prediction quality
- studying memory constrained inference
- investigating temporal localisation failures

Rather than purely optimising benchmark scores

---

# ActionFormer

ActionFormer is a transformer-based framework for temporal action localisation.

The model operates on:
- pre-extracted video features
- temporal sequence representations
- transformer based temporal modelling

and predicts:
- action boundaries
- confidence scores
- action categories

---

# Dataset

The project uses the **THUMOS14** temporal action localisation dataset.

The dataset contains:
- untrimmed videos
- temporal action annotations
- multiple action categories

Pre-extracted I3D features were used for efficient transformer based training and inference.

Due to dataset restrictions and size, the dataset is not included in this repository.

---

# Key Investigations

## Temporal IoU Analysis

The project explored how temporal IoU thresholds affect:
- true positives
- localisation accuracy
- prediction matching
- evaluation stability

---

## Error Analysis

Predictions were categorised into:
- True Positives
- Wrong Label Predictions
- Near-Miss False Positives
- Background False Positives

This helped analyse:
- localisation failures
- temporal boundary errors
- classification confusion
- over-segmentation behaviour

---

## Prediction Filtering Experiments

Experiments were conducted on:
- maximum prediction segments
- confidence filtering
- temporal overlap handling

to study how prediction filtering affects:
- mAP
- recall
- localisation quality

---

## Memory Constraints

The project was conducted under limited computational resources.

To remain computationally feasible:
- pre-extracted I3D features were used
- batch size was restricted
- temporal feature dimensions were analysed carefully

The work also explored the trade-off between:
- computational cost
- prediction quality
- temporal resolution

---

# Evaluation Metrics

Temporal localisation performance was evaluated using:
- mean Average Precision (mAP)
- temporal Intersection over Union (tIoU)
- class wise recall
- prediction matching statistics

---

# Future Improvements

Potential future work includes:
- end-to-end video feature learning
- improved temporal attention mechanisms
- boundary refinement modules
- uncertainty-aware temporal prediction
- lightweight transformer architectures

---

# Author

**Muhammad Ahmad Raza**  
Queen Mary University of London
