 pipeline {
    agent any

    tools {
        maven 'Maven 3.9.0'
    }

    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/https://github.com/DeepthiCS-cmd/pipe_test.git'
            }
        }

        stage('Build') {
            steps {
                sh 'mvn clean package'
            }
        }

        stage('Test') {
            steps {
                sh 'mvn test'
            }
        }
    }
}
