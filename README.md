# Semiconductor Wafer Defect Classification using Deep Learning

A Convolutional Neural Network (CNN) that classifies semiconductor wafer images into **8 defect categories**, built for the **IESA DeepTech Hackathon**.

**Team:** Flip Flop Squad | **Institution:** Indian Institute of Information Technology Dharwad

---

## Problem

Wafer inspection in semiconductor manufacturing is often done by eye, which is:

- Slow and labour-intensive
- Prone to human error and fatigue
- Hard to scale across production lines

## Solution

We trained a CNN that takes a wafer image and predicts its defect type automatically, giving fast and consistent inspection that does not depend on shift hours.

## Results

| Metric | Value |
| --- | --- |
| Test accuracy | [94–97%, state the exact final number] |
| Precision | [~95%, macro / weighted?] |
| Recall | [~95%, macro / weighted?] |
| Inference time | [e.g. ~__ ms per image on CPU/GPU, measured on ____] |

> Metrics are measured on a held-out test set of [N] images. See the `RESULT/` folder for the confusion matrix, training curves and sample predictions.

![Confusion matrix](RESULT/confusion_matrix.png)
<!-- Replace with your actual file name, or delete this line -->

## Defect Classes

1. [LINEAR SCRATCHES]
2. [CRACKS]
3. [PITS OR VOIDS]
4. [HOLES OR VOIDS]
5. [STAIN-OIL-DISCOLOURATION]
6. [CLEAN ]
7. [WATER STAIN]


## Dataset

- **Source:** [dataset name / link, or "provided by the hackathon organisers"]
- **Size:** [N images, with train / validation / test split]
- **Preprocessing:** [resizing, normalisation, augmentation, class balancing, etc.]

Raw data is in the `Raw data/` folder.

## Model

- **Architecture:** [e.g. 3 convolutional blocks with max pooling, followed by dense layers and softmax over 8 classes]
- **Framework:** [TensorFlow / Keras]
- **Optimiser / loss:** [e.g. Adam, categorical cross-entropy]
- **Training:** [epochs, batch size, input image size]

The trained model is saved in the `Model/` folder.

## Repository Structure

```
.
├── Model/          # Trained model files
├── Raw data/       # Wafer image dataset
├── RESULT/         # Plots, confusion matrix, sample predictions
├── wafer_defect_classification.ipynb   # Training and evaluation notebook
└── README.md
```

## How to Run

```bash
git clone https://github.com/pranavivaranasi07-dev/wafer_defect_classifier_model.git
cd wafer_defect_classifier_model
pip install -r requirements.txt
jupyter notebook wafer_defect_classification.ipynb
```

Run all cells in order to preprocess the data, train the model and reproduce the results.

## Limitations and Future Work

- Evaluated on [one dataset]; performance on images from other fabs or imaging setups is untested.
- Possible next steps: data augmentation for rare classes, transfer learning (e.g. ResNet / EfficientNet), a small web demo for uploading a wafer image, and model compression for faster inference.

## Team

- Raksha S (Team Leader)
- V Pranavi
- N Deetya
- B Lohitha

## Acknowledgements

Built for the IESA DeepTech Hackathon.
## 📧 Contact

**Email:** 25bda092@iiitdwd.ac.in  
