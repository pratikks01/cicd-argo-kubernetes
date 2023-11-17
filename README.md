# 🚀 Jenkins Pipeline for Java-based Application using Maven, SonarQube, Argo CD, and Kubernetes

![Pipeline Overview](https://github.com/pratikks01/cicd-argo-kubernetes/blob/main/images/CICD%20Block%20Diagram.png)

## Getting Started

### Prerequisites:

- 📦 Java application hosted on Git
- 🏗 Jenkins server
- 🐳 Docker, 🧰 Maven, 📊 SonarQube installed and configured
- ☸️ Kubernetes cluster
- 🎯 Argo CD

### Setup Steps:

1. **Install Jenkins Plugins:**
   - 🔄 Git
   - 🛠 Maven Integration
   - 🌐 Pipeline
   - ☁️ Kubernetes Continuous Deploy

2. **Create a Jenkins Pipeline:**
   - 🛠 Configure a new pipeline job with your Java application's Git repository URL.
   - 📝 Add a Jenkinsfile to your Git repository to define pipeline stages.

3. **Define Pipeline Stages:**
   - 🚦 Stage 1: Fetch the source code from Git.
   - 🏗 Stage 2: Compile the Java application with Maven.
   - ✅ Stage 3: Run optional unit tests with JUnit and Mockito.
   - 📊 Stage 4: Assess code quality using SonarQube.
   - 📦 Stage 5: Bundle the application into a JAR file.
   - ☁️ Stage 6: Deploy the application to a test environment using Helm.
   - 🎯 Stage 7: Execute user acceptance tests.
   - ⚙️ Stage 8: Promote the application to production using Argo CD.

4. **Configure Pipeline Stages:**
   - 🚦 Stage 1: Use Git plugin for source code checkout.
   - 🛠 Stage 2: Utilize Maven Integration for building.
   - ✅ Stage 3: Employ JUnit and Mockito plugins for testing.
   - 📊 Stage 4: Leverage SonarQube plugin for code quality analysis.
   - 📦 Stage 5: Package with Maven Integration.
   - ☁️ Stage 6: Use Kubernetes Continuous Deploy for deploying with Helm.
   - 🚀 Stage 7: Integrate Selenium or a testing framework for user acceptance tests.
   - ⚙️ Stage 8: Leverage Argo CD for production deployment.

5. **Set up Argo CD:**
   - ☸️ Install Argo CD on your Kubernetes cluster.
   - 📝 Create a Git repository for Argo CD to track changes.
   - 🧰 Develop a Helm chart for your Java application.
   - ➕ Add the Helm chart to the Argo CD-tracked Git repository.

6. **Configure Jenkins Integration with Argo CD:**
   - 🔐 Add the Argo CD API token to Jenkins credentials.
   - 🔄 Update the Jenkins pipeline to include the Argo CD deployment stage.

7. **Run the Jenkins Pipeline:**
   - ▶️ Trigger the pipeline to initiate the CI/CD process.
   - 🕵️‍♂️ Monitor stages and address any issues that arise.

This end-to-end Jenkins pipeline automates your Java application's CI/CD journey, ensuring seamless deployment using tools like SonarQube, Argo CD, and Kubernetes. 🛠️
