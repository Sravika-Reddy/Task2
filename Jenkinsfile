
pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                checkout scm
            }
        }

        stage('Build') {
            steps {
                bat 'docker build -t task2-app:latest .'
            }
        }

        stage('Test') {
            steps {
                bat 'docker run --rm task2-app:latest node --check app.js'
            }
        }

        stage('Deploy') {
            steps {
                bat '''
                    docker rm -f task2-app-container 2>NUL
                    docker run -d --name task2-app-container -p 3000:3000 task2-app:latest
                '''
            }
        }
    }
}
