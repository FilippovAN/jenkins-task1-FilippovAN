pipeline {
    agent any
    
    environment {
        APP_PORT = '9090'
    }

    stages {
        stage('Build') {
            steps {
                sh 'mvn clean install'
            }
        }

        stage('Unit Tests') {
            steps {
                sh 'mvn test'
            }
        }
    }
}
