pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                echo 'Checking source code'
            }
        }

        stage('Build Docker Image') {
            steps {
                bat 'docker --version'
                bat 'docker build -t devops-project:v1 .'
            }
        }

        stage('Test') {
            steps {
                echo 'Testing application'
            }
        }

        stage('Branch Information') {
            steps {
                echo "Current branch: ${env.BRANCH_NAME}"
            }
        }
    }
}

