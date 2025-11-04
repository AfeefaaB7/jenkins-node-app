pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/AfeefaaB7/jenkins-node-app.git'
            }
        }

        stage('Install Dependencies') {
            steps {
                sh 'npm install'
            }
        }

        stage('Build') {
            steps {
                sh 'echo "No build step yet"'
            }
        }

        stage('Test') {
            steps {
                sh 'echo "No tests yet"'
            }
        }

        stage('Deploy') {
            steps {
                sh 'echo "Deploying app..."'
                sh 'node app.js &'
            }
        }
    }

    post {
        success {
            echo '✅ Build succeeded!'
        }
        failure {
            echo '❌ Build failed!'
        }
    }
}
