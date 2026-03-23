pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git branch: 'main',
            }
        }

        stage('Check Files') {
            steps {
                bat 'dir'
            }
        }

        stage('Empty Build') {
            steps {
                bat 'echo Empty Jenkins build successful > build-report.txt'
                bat 'type build-report.txt'
            }
        }
    }

    post {
        success {
            echo 'Pipeline completed successfully'
        }
        failure {
            echo 'Pipeline failed'
        }
    }