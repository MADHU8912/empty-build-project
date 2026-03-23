pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/YOUR_USERNAME/empty-build-project.git'
            }
        }

        stage('Check Files') {
            steps {
                sh 'ls'
            }
        }

        stage('Empty Build') {
            steps {
                sh 'echo Empty build success'
            }
        }
    }
}
