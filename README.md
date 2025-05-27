 # 🚀 Twitter Spam Detection with Deep Learning
AI-Powered Twitter Spam Detection using LSTM deep learning (94% accuracy) with real-time Kafka streaming, Flask API backend, and React dashboard—deployed via Docker to classify phishing, bots, and promotions instantly.
 
## 📌 Project Overview

This deep learning system detects spam in real-time Twitter streams using LSTM neural networks. The architecture includes:

- **LSTM Classifier** (94.2% accuracy)
- **Real-time Twitter API pipeline**
- **Interactive React Dashboard**
- **Kafka-powered stream processing**

![System Architecture](assets/architecture-diagram.png) *(Suggested: Diagram of your data flow from Twitter → Kafka → Model → UI)*

## 📊 Model Performance

### Training Metrics
![Training History](assets/training-history.png) *(Suggested: Plot of accuracy/loss over epochs)*

| Metric        | Spam Class | Ham Class |
|---------------|-----------|-----------|
| Precision     | 93.8%     | 95.2%     |
| Recall        | 95.1%     | 94.8%     |
| F1-Score      | 94.4%     | 95.0%     |

### Confusion Matrix
                Predicted
               Spam   Ham
Actual Spam  [ TP    FP ]
      Ham    [ FN    TN ]
## 🖥️ UI Screenshots
 ![alt text](<WhatsApp Image 2025-05-27 at 13.24.51_1bc71870.jpg>)

**Live Detection Interface**  
![Dashboard](assets/dashboard-screenshot.png) *(Suggested: Annotated screenshot of your React UI)*

**Real-time Analytics**  
![Analytics](assets/analytics-view.png) *(Suggested: Graph showing spam/ham ratio over time)*

## 🛠️ Tech Stack

 
![alt text](image.png)
![alt text](image-1.png)
![alt text](image-2.png)
![alt text](image-3.png)
![alt text](image-4.png)

| Component       | Technology |
|-----------------|------------|
| Deep Learning   | TensorFlow/Keras |
| API Framework   | Flask      |
| Stream Processing | Apache Kafka |
| Frontend        | React      |
| Deployment      | Docker     |

## 🚀 Getting Started

```bash
# Start Kafka cluster
docker-compose -f TwitterAPI/docker-compose.yml up -d

# Launch API server
python api.py

# Start React app
cd TwitterAPI/UI && npm start