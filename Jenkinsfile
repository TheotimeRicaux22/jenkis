pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                bat 'echo Build OK'
            }
        }

        stage('Test') {
            steps {
                bat 'echo Tests OK'
            }
        }
    }

    post {
        always {
            echo 'This will always run'
        }
        success {
            echo 'This will run only if successful'
        }
        failure {
            echo 'This will run only if failed'
        }
    }
}
