pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/MADHU8912/empty-build-project.git'
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
<<<<<<< HEAD
}
=======
}
>>>>>>> f63e61d6953711a8d19c518d144eb638124752cd
