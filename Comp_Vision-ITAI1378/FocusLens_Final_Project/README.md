## **FocusLens**

**Real-Time User Engagement Monitoring System**

**FocusLens** is a computer vision application designed to monitor user alertness and presence in real-time during online lectures. It utilizes a hybrid architecture combining **MediaPipe Face Mesh** for geometric tracking and a **Support Vector Machine (SVM)** for pattern recognition to classify user status as *Attentive*, *Drowsy*, or *Absent*.

**Author:** Haamid Iman

**Course:** ITAI 1378
-----

### **Features**

  * **Hybrid Detection Logic:**
      * **Geometric (MediaPipe):** Instantly detects "Absent" state and localizes facial landmarks robust to head rotation.
      * **Machine Learning (SVM):** Analyzes pixel patterns of cropped eyes to distinguish between "Drowsy" and "Attentive" states with high accuracy.
  * **Privacy-Centric:** Processes video feeds locally (or in-session) without sending video data to external servers.
  * **Lightweight:** Designed to run efficiently on CPU without requiring heavy GPU resources.

-----

### **System Architecture**

The system processes video frames through the following pipeline:

1.  **Input:** Webcam Frame.
2.  **Face Detection:** MediaPipe scans for a face.
      * *No Face Found* $\rightarrow$ **Status: ABSENT** (Stop processing).
3.  **ROI Extraction:** If face is found, landmarks are used to crop the Left and Right Eye regions (32x32px).
4.  **Inference:** Cropped eye images are flattened and passed to the pre-trained SVM classifier.
5.  **Logic Gate:**
      * If *Left Eye* = Drowsy **AND** *Right Eye* = Drowsy $\rightarrow$ **Status: DROWSY**.
      * Otherwise $\rightarrow$ **Status: ATTENTIVE**.

-----

### **Installation**

1.  **Clone the Repository**

    ```bash
    git clone https://github.com/yourusername/FocusLens.git
    cd FocusLens
    ```

2.  **Install Dependencies**
    Create a `requirements.txt` file with the following, then install:

    ```bash
    pip install opencv-python numpy pandas mediapipe scikit-learn matplotlib joblib
    ```

-----

### **Usage Guide**

#### **Step 1: Build Your Dataset**

Run the data collection script to capture training images. This script crops eye regions automatically.

  * Set label to `"Attentive"`, look at the screen, and run.
  * Set label to `"Drowsy"`, close/droop eyes, and run.
  * *Output:* Images saved to `dataset_eyes/Attentive` and `dataset_eyes/Drowsy`.

#### **Step 2: Train the Model**

Run the training script to generate your "brain" (`eye_svm_model.pkl`).

  * Loads images from the dataset.
  * Resizes to 32x32 grayscale.
  * Trains a Linear SVM.
  * Outputs accuracy metrics and saves the `.pkl` file.

#### **Step 3: Run FocusLens**

Execute the main inference script.

  * Loads `eye_svm_model.pkl`.
  * Accesses webcam.
  * Displays real-time status overlay (Green/Red/Blue indicators).

-----

### **Project Structure**

```text
FocusLens/
├── dataset_eyes/          # Raw training data (generated)
│   ├── Attentive/
│   └── Drowsy/
├── models/
│   └── eye_svm_model.pkl  # Trained SVM classifier
├── src/
│   ├── 01_data_collection.py
│   ├── 02_train_model.py
│   └── 03_main_inference.py
├── README.md
└── requirements.txt
```

-----

### **Future Improvements**

  * **Temporal Smoothing:** Add a rolling buffer (deque) to average predictions over 5 frames to prevent flickering.
  * **Yawn Detection:** Integrate mouth aspect ratio (MAR) to detect yawning as a secondary drowsiness indicator.
  * **Local Deployment:** Port from Google Colab (JS-based camera) to native local Python (`cv2.VideoCapture`) for higher FPS.

-----
