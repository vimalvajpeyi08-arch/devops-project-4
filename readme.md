# 🚀 CI/CD Pipeline with GitHub Actions & Docker

A fully automated CI/CD pipeline built for DevOps internship evaluation. This project automates code testing, container building, and deployment using GitHub Actions and Docker Hub without requiring paid cloud infrastructure.

---

## 📌 Project Overview
* **Objective:** Set up a full CI/CD pipeline that builds a Docker image, runs automated tests, and deploys locally.
* **Domain:** DevOps Engineering
* **Platform:** GitHub Actions, Docker Hub, Python Flask

---

## 🛠️ Tools & Technologies Used
* **Version Control:** Git & GitHub
* **CI/CD Orchestration:** GitHub Actions
* **Containerization:** Docker & Docker Hub
* **Application Framework:** Python Flask & PyTest

---

## 📂 Project Structure
```text
devops-project-4/
│
├── .github/
│   └── workflows/
│       └── main.yml        # CI/CD Pipeline workflow configuration
├── app.py                  # Python Flask web application
├── requirements.txt        # Application dependencies
├── test_app.py             # Automated unit tests using PyTest
└── Dockerfile              # Multi-stage containerization blueprint
```

---

## ⚙️ Steps Involved in Building the Project
1. **Application Development:** Built a lightweight Python Flask service along with unit testing scripts (`test_app.py`).
2. **Containerization:** Created an optimized `Dockerfile` to containerize the application environment.
3. **Pipeline Configuration:** Set up GitHub Actions workflow (`.github/workflows/main.yml`) to trigger automatically on code push.
4. **Automated Testing & Build:** Configured the pipeline to run PyTest, build the Docker image, and push it directly to Docker Hub using repository secrets (`DOCKER_USERNAME` & `DOCKER_PASSWORD`).
5. **Local Deployment:** Pulled and ran the container image locally to verify runtime execution.

---

## 🚀 How to Run Locally

1. **Clone the repository:**
```bash
git clone https://github.com/vimalvajpeyi08-arch/devops-project-4.git
cd devops-project-4
```

2. **Pull and run the image from Docker Hub:**
```bash
docker run -p 5000:5000 vimalvajpeyi08/devops-demo-app:latest
```

3. **View the Application:**
Open your browser and navigate to:
👉 `http://localhost:5000`

---

## 📸 Deliverables & Proof of Execution
* **GitHub Repository:** Public repo containing workflow configurations.
* **Docker Image:** Published on Docker Hub under `vimalvajpeyi08/devops-demo-app:latest`.
* **CI/CD Results:** Verified via GitHub Actions green workflow run status checks.
* **App Preview:** Successfully verified runtime view at `http://localhost:5000`.