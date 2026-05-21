pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Stage 1: Build - Building the code using Maven.'
                echo 'Tool: Maven - a build automation tool for Java projects that compiles source code and packages it into a JAR/WAR file.'
            }
        }
        stage('Unit and Integration Tests') {
            steps {
                echo 'Stage 2: Unit and Integration Tests'
                echo 'Running unit tests to verify individual components work correctly.'
                echo 'Running integration tests to verify components work together.'
                echo 'Tools: JUnit for unit testing, Selenium for integration testing.'
            }
        }
        stage('Code Analysis') {
            steps {
                echo 'Stage 3: Code Analysis'
                echo 'Analysing code quality and ensuring it meets industry standards.'
                echo 'Tool: SonarQube - performs static code analysis to detect bugs, code smells, and security vulnerabilities.'
            }
        }
        stage('Security Scan') {
            steps {
                echo 'Stage 4: Security Scan'
                echo 'Scanning the code for known security vulnerabilities.'
                echo 'Tool: OWASP Dependency-Check - scans project dependencies for known CVEs.'
            }
        }
        stage('Deploy to Staging') {
            steps {
                echo 'Stage 5: Deploy to Staging'
                echo 'Deploying the application to a staging server for further testing.'
                echo 'Tool: AWS CLI - used to deploy the application to an AWS EC2 instance.'
            }
        }
        stage('Integration Tests on Staging') {
            steps {
                echo 'Stage 6: Integration Tests on Staging'
                echo 'Running integration tests on the staging environment to validate production-like behaviour.'
                echo 'Tool: Selenium - automates browser-based testing against the staging server.'
            }
        }
        stage('Deploy to Production') {
            steps {
                echo 'Stage 7: Deploy to Production'
                echo 'Deploying the application to the production server.'
                echo 'Tool: AWS CLI - used to deploy the final build to an AWS EC2 production instance.'
            }
        }
    }
}
