pipeline {
    agent any

    stages {
        // ... The Build stage is here ...
        stage('Build') {
            steps {
                sh 'npm install'
            }
        }

        // NEW: We add the Test stage here
        stage('Test') {
            steps {
                // This command runs a script that checks if the app is working
                sh './jenkins/scripts/test.sh'
            }
        }
    }
}