pipeline {
    agent any

    stages {
        stage('Check Files') {
            steps {
                bat 'dir'
            }
        }

        stage('Empty Build') {
            steps {
                bat 'echo Empty build success'
            }
        }
    }
}