# 🏥 Colorectal Cancer Patient Survival Prediction

An end-to-end MLOps project for predicting colorectal cancer patient survival using machine learning, with comprehensive experiment tracking, pipeline orchestration, and deployment automation.

## 🎯 Project Overview

This project implements a complete machine learning pipeline for colorectal cancer survival prediction, showcasing modern MLOps practices including experiment tracking with MLflow, containerization with Docker, and orchestration using Kubeflow on a local Kubernetes cluster.

## ✨ Key Features

- **MLflow Integration with DagsHub**: Complete experiment tracking and model versioning
- **Local Kubernetes Cluster**: Production-grade infrastructure on your local machine
- **Kubeflow Pipelines**: Automated ML workflow orchestration
- **Docker Containerization**: Consistent deployment across environments
- **Data Versioning**: Track datasets and code changes throughout the project lifecycle
- **End-to-End Pipeline**: From data processing to model deployment

## 🏗️ Architecture & Workflow

```
Project Setup → Jupyter Notebook Testing → Data Processing
                                                ↓
User App ← Dockerization ← Pipeline Making ← Model Training
    ↓                            ↓                ↓
Deployment   ← Kubeflow Setup ← Data/Code Versioning ← Experiment Tracking
```

## 🛠️ Technologies Used

- **ML Framework**: Scikit-learn, Pandas, NumPy
- **Experiment Tracking**: MLflow + DagsHub
- **Orchestration**: Kubeflow Pipelines
- **Containerization**: Docker, DockerHub
- **Infrastructure**: Kubernetes (local cluster)
- **Version Control**: Git, DVC (Data Version Control)

## 📊 Dataset

This project uses colorectal cancer patient data to predict survival outcomes. The dataset includes various clinical and pathological features that influence patient prognosis.

## 🚀 Getting Started

### Prerequisites

- Python 3.8+
- Docker Desktop
- Kubernetes (Minikube or Docker Desktop with K8s enabled)
- kubectl CLI
- Git

### Installation

1. Clone the repository
```bash
git clone https://github.com/imchandanmohan/Colorectal-Cancer-Survival-Prediction.git
cd Colorectal-Cancer-Survival-Prediction
```

2. Install dependencies
```bash
pip install -r requirements.txt
```

3. Configure MLflow with DagsHub
```bash
# Set environment variables
export MLFLOW_TRACKING_URI=your_dagshub_uri
export MLFLOW_TRACKING_USERNAME=your_username
export MLFLOW_TRACKING_PASSWORD=your_password
```

### Running the Project

1. **Data Processing**: Process and prepare the dataset
2. **Model Training**: Train models with experiment tracking
3. **Kubeflow Pipeline**: Set up and run automated pipelines
4. **Deployment**: Deploy the model using Docker and Kubernetes

## 📁 Project Structure

```
├── data/                   # Dataset files
├── notebooks/             # Jupyter notebooks for experimentation
├── src/                   # Source code
│   ├── data_processing/  # Data preparation scripts
│   ├── model_training/   # Training scripts
│   └── pipeline/         # Kubeflow pipeline definitions
├── docker/               # Dockerfiles
├── kubernetes/           # K8s manifests
├── mlruns/              # MLflow tracking data
└── README.md
```

## 🔬 Experiment Tracking

All experiments are tracked using MLflow and stored on DagsHub, providing:
- Model parameters and metrics
- Artifact storage
- Model versioning
- Experiment comparison

## 🐳 Docker & Kubernetes

The project includes:
- Dockerfiles for containerizing the application
- Kubernetes manifests for deployment
- Kubeflow pipeline definitions for automated workflows

## 📈 Use Cases

- **Clinical Decision Support**: Assist healthcare providers in treatment planning
- **Risk Stratification**: Identify high-risk patients for targeted interventions
- **Research Applications**: Enable survival analysis for clinical research
- **Healthcare Analytics**: Support population health management initiatives

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## 📝 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 👤 Author

**Chandan Mohan**
- GitHub: [@imchandanmohan](https://github.com/imchandanmohan)

## 🙏 Acknowledgments

- DagsHub for MLflow hosting
- Kubeflow community for orchestration tools
- Healthcare datasets contributors

---

⭐ If you find this project helpful, please consider giving it a star!