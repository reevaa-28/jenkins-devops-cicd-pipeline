**# Jenkins DevOps CI/CD Pipeline**



**A Maven-based Java project integrated with Jenkins to demonstrate a complete CI/CD delivery pipeline.**



**## CI/CD Pipeline**



**The Jenkins pipeline consists of six stages:**



**1. DevCompile – Compiles the Java application**

**2. CodeReview – Performs PMD code analysis**

**3. UnitTest – Executes unit tests**

**4. MetricCheck – Generates code coverage metrics**

**5. Package – Packages the application**

**6. Deploy – Executes the deployment stage**



**### Pipeline Flow**



**DevCompile → CodeReview → UnitTest → MetricCheck → Package → Deploy**



**## Technologies Used**



**- Java**

**- Apache Maven**

**- Jenkins**

**- Git**

**- GitHub**

**- PMD**

**- Cobertura**

**- JUnit**



**## Project Structure**



**```text**

**jenkins-devops-cicd-pipeline/**

**├── src/**

**├── pom.xml**

**├── Jenkinsfile**

**├── .gitignore**

**└── README.md**

