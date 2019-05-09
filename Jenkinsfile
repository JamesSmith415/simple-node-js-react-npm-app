pipeline {
    agent any
    environment {
        CI = 'true' 
    }
    stages {
        stage('Build') {
            steps {
                bash 'npm install'
            }
        }
        stage('Test') { 
            steps {
                bash './jenkins/scripts/test.sh' 
            }
        }
    }
}