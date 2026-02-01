pipeline {
    agent {
        docker {
            image 'node:18-alpine'
        }
    }

    stages {
        stage('Install') {
            steps {
                sh 'node -v'
                sh 'npm -v'
                sh 'npm install'
            }
        }

        stage('Build') {
            steps {
                sh 'npm run build'
            }
        }
    }
}
