
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
                bat 'docker --version'
                bat 'docker build -t devops-project:v1 .'
            }
        }

        stage('Test') {
            steps {
                echo 'Testing application'
                bat 'docker images'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deployment stage completed'
            }
        }
    }

    post {
        success {
            echo 'Pipeline completed successfully!'
        }
        failure {
            echo 'Pipeline failed. Check console output.'
        }
    }
}


