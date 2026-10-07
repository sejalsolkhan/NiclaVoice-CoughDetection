# NiclaVoice-CoughDetection
Cough detection using Edge Impulse on Arduino Nicla Voice (NDP120)
# Nicla Voice Cough Detection V6

This project uses Edge Impulse to detect coughs using the Arduino Nicla Voice and its Syntiant NDP120 processor.

## Model

- Classification: Cough vs. Non-cough
- Audio sampling rate: 16 kHz
- Window size: 968 ms
- Feature extraction: Syntiant log-bin (NDP120)
- Deployment: Arduino Nicla Voice

## Model Testing Results

- Held-out test accuracy: **89.21%**
- Cough correctly classified: **89.5%**
- Non-cough correctly classified: **88.9%**
- Non-cough misclassified as cough: **7.4%**
- AUC: **0.91**
- Weighted F1 score: **0.91**

## Deployment

The firmware was built using Edge Impulse and successfully flashed onto the Arduino Nicla Voice.

After flashing the firmware, live cough detections can be viewed using:

`edge-impulse-run-impulse --raw`

The board reports detected cough events as:

`Match: NN0:cough`
