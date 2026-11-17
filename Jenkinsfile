pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git branch: 'main',
                    url: 'https://github.com/KARTIK3319/DevOps-Configuration.git'
            }
        }

        stage('Build') {
            steps {
                bat 'echo Build completed'
            }
        }

        stage('Test') {
            steps {
                bat 'echo Test completed'
            }
        }
    }
}
