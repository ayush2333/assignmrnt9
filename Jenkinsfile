
pipeline {
    agent any

    stages {
        stage('Build Docker Image') {
            steps {
                script {
                    bat 'docker build -t myapp:latest .'
                }
            }
        }
        stage('Build and Run Docker Container') {
            steps {
                script {
                    bat 'docker run -d --name myapp-container -p 5000:5000 myapp:latest'
                }
            }
        }
    }
}
