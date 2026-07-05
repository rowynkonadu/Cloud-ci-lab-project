# Cloud-ci-lab-project
End to End CI/CD Pipeline
# Cloud CI/CD Lab Project

## 👨‍💻 Author
**Name**: Rowyn Konadu  
**GitHub**: https://github.com/rowynkonadu/Cloud-ci-lab-project  
**Project**: CLOUD-CI-LAB-PROJECT  
A hands-on DevOps project demonstrating a complete CI/CD pipeline using GitHub Actions and GitOps principles.

## Objective
Build, test, and deploy a Python application automatically on every push to GitHub. Simulate failures and fixes to demonstrate error handling.

## 📌 About This Project

This project demonstrates the fundamentals of modern DevOps and CI/CD practices. 

I built a fully automated pipeline using GitHub Actions that triggers on every push to the `main` branch. The pipeline checks out code, sets up the Python environment, logs build information, runs the application, and reports test status.

Key DevOps concepts covered:
- **Continuous Integration**: Automated build and test on every commit
- **GitOps**: Managing infrastructure and pipelines through Git
- **Workflow Automation**: 6-step pipeline from checkout to reporting
- **Error Handling**: Simulated failures and recovery testing

This project was built as part of my Cloud Computing Lab to gain hands-on experience with cloud-native tooling.
## Tech Stack
- **Language**: Python 3.10
- **CI/CD**: GitHub Actions
- **Version Control**: Git & GitHub
- **Methodology**: GitOps

## Project Structure

## ⚙️ CI Pipeline Breakdown
The workflow triggers on every `push` to `main` branch:

1.  **Checkout Code**: Pull latest code from repo
2.  **Setup Environment**: Install Python 3.10
3.  **Build Info**: Log build message and Python version
4.  **Execute App**: Run `app.py`
5.  **Test Report**: Confirm all tests passed

## 📊 Results

### Task : Successful Pipeline Execution
![Successful Pipeline](screenshots/success.png)
*All 6 steps completed successfully. Output from app.py is visible.*


![Recovered Pipeline](screenshots/fixed.png)
*Fixed the error, pushed the commit, and pipeline recovered to green.*

## 🧠 Key Learnings
- Configured and debugged GitHub Actions YAML workflows
- Applied GitOps: All infrastructure changes done via code commits
- Implemented automated testing and failure handling in CI
- Gained experience with cloud-native DevOps tooling

## 🚀 How to Run
```bash
git clone https://github.com/rowynkonadu/cloud-ci-lab-project
cd cloud-ci-lab-project
python app.py
