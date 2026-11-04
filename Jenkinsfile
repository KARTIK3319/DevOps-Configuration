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
                echo 'Building Docker image'
                sh 'docker build -t devops-project:v1 .'
            }
        }

        stage('Test') {
            steps {
                echo 'Application build completed'
            }
        }
    }
}