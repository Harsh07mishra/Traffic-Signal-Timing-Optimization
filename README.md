🚦 Traffic Signal Timing Optimizer — ML-Powered Smart Traffic Control System
<p align="center"> <img src="https://img.shields.io/badge/Traffic-Optimization-red?style=for-the-badge" /> <img src="https://img.shields.io/badge/Machine%20Learning-Active-blue?style=for-the-badge" /> <img src="https://img.shields.io/badge/Computer%20Vision-YOLOv8-green?style=for-the-badge" /> <img src="https://img.shields.io/badge/Python-3.10+-yellow?style=for-the-badge" /> <img src="https://img.shields.io/badge/License-MIT-orange?style=for-the-badge" /> </p> <p align="center"> <b>Traffic Signal Timing Optimizer</b> is an ML-driven system that dynamically adjusts green-light durations based on detected vehicle density, improving traffic flow and reducing congestion at intersections. </p>

🚗 YOLOv8-based vehicle detection in real time

📊 Weighted traffic scoring using car/bike/bus/truck counts

🤖 ML model to classify traffic levels (Low / Normal / High / Heavy)

⏱ Dynamic green-light duration calculation

🔄 Time-series prediction for future traffic patterns

📉 Supports optimization strategies to minimize delay and queue length

🛣 Suitable for real-world deployments & smart-city applications

🏗️ System Architecture
flowchart LR
    A[Camera Feed / Image Input] --> B[YOLOv8 Vehicle Detection]
    B --> C[Vehicle Counts (Car/Bike/Bus/Truck)]
    C --> D[Weighted Score Calculation]

    D --> E[Traffic Level Classifier (ML)]
    E --> F[Traffic Category: Low/Normal/High/Heavy]

    F --> G[Green Time Optimizer]
    C --> G

    G --> H[Optimized Signal Timing Output]
🛠️ Technology Stack
Component	Methods	Libraries
Object Detection	YOLOv8	Ultralytics, OpenCV
Traffic Level Classification	ML Models (RandomForest, XGBoost, SVM)	Scikit-Learn
Time-Series Prediction	ARIMA, Prophet, LSTM	Statsmodels, Prophet, PyTorch
Green Time Calculation	Weighted vehicle score model	NumPy, Pandas
Visualization	Heatmaps, traffic trend plots	Matplotlib, Seaborn
📊 Weighted Scoring Formula
Weighted Score = (Bike × 1) + (Car × 2) + (Bus × 5) + (Truck × 5)

Example:
10 bikes + 5 cars + 1 bus →
Score = 10×1 + 5×2 + 1×5 = 25

This score is used to:

1️⃣ Classify traffic level
2️⃣ Compute optimal green-light duration

🧮 Green Light Time Optimization
Green Time = Base Time + (Weighted Score × Scaling Factor)

Dynamic adjustment ensures minimum waiting time and smooth traffic flow.

📈 Datasets Used

Chandigarh Roads Traffic Dataset

Custom vehicle-count datasets

YOLO annotation datasets for fine-tuning

🚀 Future Enhancements

Cross-junction optimization using graph-based modeling

Reinforcement learning for adaptive control

Integration with smart signals & IoT sensors

Cultural / regional traffic pattern adaptation

Deployment on edge devices (Jetson Nano / Raspberry Pi)

Explainable AI for transparent signal decisions

🤝 Contributing

Contributions, suggestions, and improvements are welcome!
Open an issue or submit a PR to contribute.

👤 Author

Harsh Mishra
Traffic AI Research & ML Developer
Project: ML-Powered Traffic Signal Timing Optimization
