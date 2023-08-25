pipeline {
    agent any
    parameters {
        string(name: 'BRANCH', defaultValue: 'main', description: 'Branch to checkout')
    }
    options {
        skipDefaultCheckout() 
    }
    stages {
        stage('Checkout') {
            steps {
                script {
                    echo ""
                    checkout([
                        $class: 'GitSCM',
                        branches: [[name: params.BRANCH]],
                        userRemoteConfigs: [[
                            url: "${env.REPO_URL}",
                            credentialsId: "${env.CREDENTIALS_ID}"
                        ]]
                    ])
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
