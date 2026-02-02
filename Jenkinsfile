pipeline {
    agent any

    tools {
        nodejs 'node18'
    }

    stages {
        stage('Checkout SCM') {
            steps {
                checkout scm
            }
        }

        stage('Build') {
            steps {
                sh 'npm install'
                sh 'npm run build'
            }
        }

        stage('Test') {
            steps {
                sh 'npm test'
            }
        }

        stage('Deliver') {
            steps {
                echo 'Delivering application...'
                sh 'echo "Application delivered successfully"'
            }
        }
    }
}
