
pipeline {
    agent any

    stages {
        stage('Build Docker Image') {
            steps {
                script {
                    bat 'docker build -t ayush2333/assignment9 .'
                }
            }
        }
        stage('Build and Run Docker Container') {
            steps {
                script {
                    bat 'docker run -d --name ayush2333/assignment9  -p 5000:5000 '

                    bat 'docker push  ayush2333/assignment9 '
                    
                }
            }
        }
    }
}
