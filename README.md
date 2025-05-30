
# Biometric Auth System: Voice + Face Recognition

This project is a dual-modality biometric authentication system using **voice** and **face recognition**. Built with machine learning, the system provides enhanced security by verifying identity through both visual and auditory features.

## 🔐 About the Project

Traditional authentication methods like passwords or PINs are prone to theft and misuse. This system uses biometric signals — human face and voice — to validate identity, reducing risk and improving security.

The project combines:
- **Face Recognition** using computer vision and feature matching
- **Voice Recognition** using speech processing and classification
- A final **authentication decision** that confirms the user only if both inputs match the registered identity

## 🧠 Technologies Used

- **Python** & **Jupyter Notebook**
- **OpenCV** – for face detection and recognition
- **Librosa / Soundfile / PyDub** – for voice processing
- **Scikit-learn / TensorFlow / Keras** – for ML models
- **NumPy / Pandas / Matplotlib** – for data handling and visualization

## 🚀 Features

- ✅ Real-time **face capture and recognition**
- ✅ Accurate **voice feature extraction**
- ✅ Machine learning models for both modalities
- ✅ Combines both face and voice for **secure authentication**
- ✅ Can be extended to use CNNs, Siamese Networks, or speaker embedding models

## 🛠️ How It Works

1. **Data Collection**
   - Captures a person's voice and face during registration.

2. **Preprocessing**
   - Face is detected and cropped using OpenCV.
   - Voice is converted to MFCC or spectrogram features.

3. **Model Training**
   - Trains individual classifiers for face and voice.

4. **Authentication Phase**
   - Accepts live face and voice.
   - Predicts identity from both models.
   - Grants access only if both match the registered identity.

## 🧪 Example Use Case

```python
# Load image and voice sample
face = capture_face()
voice = record_voice()

# Authenticate
if authenticate_user(face, voice):
    print("Access Granted ✅")
else:
    print("Access Denied ❌")


## 💻 Installation

1. Clone this repository:

   ```bash
   git clone https://github.com/siddharth-coder8/Biometric-Auth-System.git
   cd Biometric-Auth-System
   ```

2. Install required packages:
   *(Create a virtual environment if needed)*

   ```bash
   pip install -r requirements.txt
   ```

3. Run the Jupyter Notebook:

   ```bash
   jupyter notebook biometric-ml-auth.ipynb
   ```

## 📌 Future Improvements

* [ ] Deploy as a desktop or web app
* [ ] Use deep learning (e.g., FaceNet, SpeakerNet)
* [ ] Add anti-spoofing protection
* [ ] Store biometric profiles securely (e.g., encryption, hashing)

## 👨‍💻 Author

**Siddharth Shah**
 [SVECTOR](https://www.svector.co.in)
Founder of SVECTOR

## 📜 License

This project is licensed under the MIT License. Feel free to modify and use it for your own purposes.

---

> **Biometric-Auth-System** — Securing access with the power of voice and vision.
