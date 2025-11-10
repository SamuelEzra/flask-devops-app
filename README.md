# Flask DevOps Application

A Flask web application demonstrating DevOps practices with GitHub Actions CI/CD, Docker containerization, and automated deployments.

## 📁 Repository Structure

flask-devops-app/
├── .github/ # GitHub Actions workflows
├── .dockerignore # Docker ignore rules
├── .gitignore # Git ignore rules
├── Dockerfile # Docker configuration
├── README.md # Project documentation
├── app.py # Main Flask application
└── requirements.txt # Python dependencies


## 🚀 Features

- **Flask Web Framework** - Lightweight Python web application
- **Docker Containerization** - Ready for container deployment
- **GitHub Actions CI/CD** - Automated testing and deployment pipeline
- **Production Ready** - Proper dependency management and configuration
- **DevOps Best Practices** - Includes proper .gitignore and .dockerignore

## 🛠️ Quick Start

### Prerequisites
- Python 3.8+
- Docker (optional)
- Git

### Local Development

1. **Clone the repository**
   ```bash
   git clone https://github.com/SamuelEzra/flask-devops-app.git
   cd flask-devops-app

2. **Set up virtual environment**
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

3. **Install dependencies**
```bash
pip install -r requirements.txt
```

4. **Run the application**
```bash
python app.py
```

Access at: `http://localhost:5000`

### Docker Development

```bash
# Build the Docker image
docker build -t flask-devops-app .

# Run the container
docker run -p 5000:5000 flask-devops-app
```

Project Files

app.py - Flask Application

The main Flask web application containing routes and business logic.

requirements.txt - Dependencies

Python package dependencies for the application.

Dockerfile - Container Configuration

Docker configuration for building the application container.

.gitignore - Git Ignore Rules

venv/ - Python virtual environment
__pycache__/ - Python cache files
*.pyc - Compiled Python files
.dockerignore - Docker Ignore Rules

Specifies files to exclude from Docker builds for optimal image size.

.github/ - GitHub Actions

CI/CD workflows for automated testing and deployment.


### GitHub Actions CI/CD

This repository includes GitHub Actions workflows for:

- Continuous Integration: Automated testing on push and pull requests
- Continuous Deployment: Automatic deployment to chosen platforms
- Multi-environment Testing: Testing across different Python versions
- Code Quality Checks: Linting and formatting validation


### Docker Deployment

#### Build the Image

```bash
docker build -t samueleza/flask-devops-app .
```

### Run the Container
```bash
docker run -d -p 5000:5000 --name flask-app samueleza/flask-devops-app
```
