 pipeline {
    agent any

    tools {
        maven 'Maven_Home 3.9.10'
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
