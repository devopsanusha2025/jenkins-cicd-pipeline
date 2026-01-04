pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                git branch: 'main',
                    url: 'https://github.com/devopsanusha2025/jenkins-cicd-pipeline.git'
            }
        }

        stage('Build') {
            steps {
                echo 'Building the application...'
            }
        }

        stage('Test') {
            steps {
                echo 'Running unit tests...'
            }
        }

        stage('Docker Build') {
            steps {
                echo 'Building Docker image...'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying application to environment...'
            }
        }
    }

    post {
        success {
            echo 'Pipeline executed successfully!'
        }
        failure {
            echo 'Pipeline failed!'
        }
    }
}
