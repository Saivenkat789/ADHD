Pose Estimation–Enabled Behavioral Monitoring System for ADHD Diagnosis in Children

A machine learning and computer vision–based system that uses human pose estimation and behavioral monitoring to assist in the diagnosis of ADHD (Attention Deficit Hyperactivity Disorder) in children. The project combines OpenCV pose detection, Support Vector Machine (SVM) classification, and a Tkinter GUI for interactive testing on images and videos.

📌 Features
Upload and preprocess ADHD pose dataset
Train and test an SVM classification model
Human pose estimation using OpenCV DNN
ADHD prediction from:
Images
Videos
Confusion matrix and performance metrics visualization
User-friendly GUI using Tkinter
🛠️ Technologies Used
Python
OpenCV
Tkinter
NumPy
Pandas
Scikit-learn
Matplotlib
Seaborn
📂 Project Structure
Project/
│── Main.py
│── Models/
│   ├── pose_deploy_linevec.prototxt
│   └── pose_iter_440000.caffemodel
│── ADHDDataset/
│── images/
│── videos/
│── README.md
⚙️ Installation
1️⃣ Clone the Repository
git clone https://github.com/your-username/adhd-pose-monitoring.git
cd adhd-pose-monitoring
2️⃣ Install Dependencies
pip install numpy pandas matplotlib seaborn scikit-learn opencv-python
▶️ Running the Project

Run the main Python file:

python Main.py
🧠 Working Process
Step 1: Upload Dataset
Load the ADHD pose dataset CSV file.
Step 2: Preprocess Dataset
Shuffle dataset
Normalize features using StandardScaler
Step 3: Split Dataset
80% training data
20% testing data
Step 4: Train Model
SVM classifier with RBF kernel is trained.
Step 5: Detect ADHD
Pose estimation extracts body keypoints.
Features are passed to the trained model.
System predicts:
Normal
ADHD Disease
📊 Evaluation Metrics

The project calculates:

Accuracy
Precision
Recall
F1-Score
Confusion Matrix
🖼️ Pose Estimation

The system uses OpenCV DNN pose estimation model with:

pose_deploy_linevec.prototxt
pose_iter_440000.caffemodel

Detected body joints are connected using predefined pose pairs for skeleton visualization.

📸 Image Detection
Upload an image
Detect human pose
Predict ADHD behavior
Display skeleton and prediction result
🎥 Video Detection
Upload a video
Analyze multiple frames
Predict ADHD based on pose behavior patterns
📈 Machine Learning Model
Support Vector Machine (SVM)
svm.SVC(kernel="rbf", C=12, probability=True, gamma="auto")

Used for behavioral classification after pose feature extraction.

🔍 Future Enhancements
Deep learning–based ADHD detection
Real-time webcam monitoring
Higher accuracy with larger datasets
Web-based deployment
Multi-person pose tracking
👨‍💻 Author

Sai Venkatesh

📜 License

This project is developed for educational and research purposes.
