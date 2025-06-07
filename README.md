This project develops a deep learning-based solution to automate the scoring process in shooting sports by detecting bullet holes and calculating scores from scanned shooting target cards. Traditional scoring is time-consuming and prone to human error, and this work addresses these limitations by using state-of-the-art object detection models.

🔍 Objective
To improve the accuracy, speed, and reliability of scoring in shooting sports by automating bullet hole detection and score computation using deep learning techniques.

💡 Motivation
Manual scoring methods are:

Prone to human error

Time-intensive

Not scalable for large competitions

Our system replaces traditional methods with a robust, real-time machine learning model for accurate score assessment.

🧠 Models Explored
We experimented with three models for bullet hole detection and scoring:

Model	Accuracy/Precision	Notes
YOLOv9	91% precision, 89% recall	Best performance, real-time, anchor-free detection
AdaBoost	82.3% accuracy	Lightweight, but struggles with clustered shots
Mask R-CNN	68% accuracy	High segmentation capability, but poor performance due to small dataset

📦 Dataset
Collected from Manav Rachna Shooting Arena, Faridabad, India

176 scanned images: 88 inner ring, 88 outer ring

Format: .png, resolution standardized to 640×640

Validation .csv includes:

Image name

Ring category (Inner/Outer)

Expert-assigned score

📊 Methodology
Preprocessing: Images resized and labeled

Training: Data split into train/validation/test sets

Model Comparison: Evaluated via precision, recall, and detection accuracy

Scoring: Bullet hole location mapped to scoring rings

<!-- Replace with actual path if available -->

🔬 Results
YOLOv9 demonstrated the highest performance in both detection accuracy and score estimation.

Precision-Recall curves confirm YOLOv9’s robustness in varying conditions.

Sample Detection:

<!-- Replace with actual path -->

🧪 Technologies Used
Python

OpenCV

PyTorch

YOLOv9

Mask R-CNN (Torchvision)

Scikit-learn (for AdaBoost)

📈 Future Work
Incorporate real-time video feed support

Expand to support different target card formats

Improve detection under variable lighting and occlusion

📚 Citation
If you use this work, please cite:

Girija R., Kaur M., Singh M., Gera P., Panker S., Yaduvanshi M.
Target Recognition and Scoring Automation: A Machine Learning Perspective, 2025

📎 References
Refer to the full list of citations in the docs/references.md file or the research paper attached.

👤 Contributors
Pratham Gera

Manpreet Kaur

R. Girija

Maneesha Singh

Sanchit Panker

Mohan Yaduvanshi
