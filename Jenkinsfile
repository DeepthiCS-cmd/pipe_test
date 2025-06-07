 pipeline {
    agent any

    tools {
        maven 'Maven 3.6.3'
    }

    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/your-user/your-java-project.git'
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
