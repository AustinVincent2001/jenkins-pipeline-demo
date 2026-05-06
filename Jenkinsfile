pipeline {
    agent any

    environment {
        STAGING_ENV = "AWS EC2 - Staging"
        PRODUCTION_ENV = "AWS EC2 - Production"
    }

    stages {

        stage('Build') {
            steps {
                echo "Build Stage: Compile and package the application using Maven (build automation tool)"
            }
        }

        stage('Unit and Integration Tests') {
            steps {
                echo "Testing Stage: Run unit tests using JUnit and integration tests using Selenium"
            }
        }

        stage('Code Analysis') {
            steps {
                echo "Code Analysis Stage: Analyse code quality using SonarQube"
            }
        }

        stage('Security Scan') {
            steps {
                echo "Security Scan Stage: Scan application for vulnerabilities using OWASP ZAP"
            }
        }

        stage('Deploy to Staging') {
            steps {
                echo "Deploy Stage: Deploy application to staging environment (${STAGING_ENV}) using AWS EC2"
            }
        }

        stage('Integration Tests on Staging') {
            steps {
                echo "Staging Test Stage: Perform integration testing on staging using Selenium"
            }
        }

        stage('Deploy to Production') {
            steps {
                echo "Production Stage: Deploy application to production environment (${PRODUCTION_ENV}) using AWS EC2"
            }
        } 
        stage('Deploy to new Production') {
            steps {
                echo "Production Stage: new Deploy application to production environment (${PRODUCTION_ENV}) using AWS EC2"
            }
        }
    }
}
