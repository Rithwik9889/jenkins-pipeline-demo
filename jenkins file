pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo 'Stage 1: Build - Compiling and packaging code using Maven.'
                echo 'Tool: Maven'
            }
        }
        stage('Unit and Integration Tests') {
            steps {
                echo 'Stage 2: Unit & Integration Tests - Running JUnit unit tests and Selenium integration tests.'
                echo 'Tools: JUnit, Selenium'
            }
        }
        stage('Code Analysis') {
            steps {
                echo 'Stage 3: Code Analysis - Analysing code quality with SonarQube.'
                echo 'Tool: SonarQube'
            }
        }
        stage('Security Scan') {
            steps {
                echo 'Stage 4: Security Scan - Scanning for vulnerabilities with OWASP Dependency-Check.'
                echo 'Tool: OWASP Dependency-Check'
            }
        }
        stage('Deploy to Staging') {
            steps {
                echo 'Stage 5: Deploy to Staging - Deploying application to AWS EC2 staging instance.'
                echo 'Tool: AWS EC2'
            }
        }
        stage('Integration Tests on Staging') {
            steps {
                echo 'Stage 6: Integration Tests on Staging - Running JMeter tests on staging environment.'
                echo 'Tool: JMeter'
            }
        }
        stage('Deploy to Production') {
            steps {
                echo 'Stage 7: Deploy to Production - Deploying to production AWS EC2 via AWS CodeDeploy.'
                echo 'Tool: AWS CodeDeploy'
            }
        }
    }
}
