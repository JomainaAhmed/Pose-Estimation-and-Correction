# Form Correctness Detection Using Pose Estimation

A computer vision–based system for analysing fitness exercise form using **human pose estimation**. The project extracts body keypoints from video input and evaluates posture correctness through **rule-based biomechanical logic** and **machine learning–assisted phase detection**.

Developed as part of an **AI Intern Onsite Task (Computer Vision & AI)** with emphasis on interpretability, real-time feedback, and practical usability.

---

## 🎯 Objectives

- Detect human body keypoints from exercise videos  
- Analyse posture using geometric and rule-based logic  
- Identify exercise phases and count repetitions  
- Provide frame-wise real-time feedback  
- Demonstrate practical use of pose estimation techniques  

---

## 🏋️ Exercises Analysed

- Squat  
- Deadlift  
- Bench Press  

These exercises involve complex multi-joint movements where correct posture is critical.

---

## 🛠 Technologies Used

- **Python**
- **MediaPipe Pose** – Human pose and landmark detection  
- **OpenCV** – Video processing and visual feedback  
- **Scikit-learn** – Exercise phase classification  
- **NumPy** – Angle and geometric calculations  
- **Pandas** – Pose data handling  
- **Matplotlib** – Analysis and debugging visualizations  

---

## ⚙️ How It Works

1. Capture video frames using OpenCV  
2. Extract 33 body landmarks per frame with MediaPipe Pose  
3. Compute joint angles and relative alignments  
4. Apply rule-based posture validation  
5. Detect exercise phases  
6. Count repetitions using phase transitions  
7. Display real-time feedback on video frames  

---

## 📏 Posture Evaluation Rules

### Joint Angle Control
Validates angles at key joints such as hips, knees, shoulders, and elbows.

### Joint Alignment
Monitors alignment between important joint pairs (e.g., wrist–shoulder, hip–shoulder).

### Back Posture & Symmetry
Detects forward lean, imbalance, or rounding of the back using shoulder–hip positioning.

Rules are applied **frame-wise** to ensure interpretable and explainable feedback.

---

## 🚀 Getting Started

### Clone the Repository
```bash
git clone <repository-url>
cd Pose-Estimation-for-Fitness-Exercise-Analysis
```

## Set Up Virtual Environment
python -m venv venv
venv\Scripts\activate      # Windows

## Install Dependencies
pip install -r requirements.txt

## Run the Application
python Model_Predictions.py

## 🎥 Output

- Pose landmarks overlay on video
- Exercise phase indicator
- Repetition counter
- Text-based posture feedback

## ⚠️ Limitations

- Assumes a single person per frame
- Fixed camera angle recommended for best accuracy

## 🔮 Future Improvements

- Multi-person pose tracking
- Temporal smoothing of pose data
- MLFlow integration
- Web or mobile deployment
