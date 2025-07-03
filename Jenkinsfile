pipeline {
    agent any

    stages {
        stage('Clone') {
            steps {
                git 'https://github.com/AgengCDB/jenkins-pipeline-demo.git'
            }
        }
        stage('Build') {
            steps {
                echo '✅ Code cloned. Simulating build step...'
            }
        }
        stage('Test') {
            steps {
                echo '🧪 Running tests (simulated)...'
            }
        }
    }

    post {
        success {
            echo '🎉 Build and test succeeded!'
        }
        failure {
            echo '❌ Build failed!'
        }
    }
}
