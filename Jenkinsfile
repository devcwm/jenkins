pipeline {
    agent any
    environment {
        REPO_URL = credentials('REPO_URL')
        CREDENTIALS_ID = credentials('CREDENTIALS_ID')
    }
    parameters {
        string(name: 'BRANCH', defaultValue: 'main', description: 'Branch to checkout')
    }
    stages {
        stage('Checkout') {
            steps {
                script {
                    echo "${REPO_URL}"
                }
            }
        }
        stage('Build') {
            steps {
                // Your build steps here
                echo "Hello"
            }
        }
        stage('Test') {
            steps {
                // Your test steps here
                echo "Hello"
            }
        }
        stage('Deploy') {
            steps {
                // Your deployment steps here
                echo "Hello"
            }
        }
    }
    post {
        always {
            // Post-build actions
            echo "Hello"
        }
    }
}
