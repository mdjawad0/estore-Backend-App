pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                // Get some code from a GitHub repository
                git 'https://github.com/mdjawad0/estore-Backend-App.git'

                // Run Maven Wrapper Commands
                sh "./mvnw compile"

                echo 'Building the Project with Maven Wrapper compile'
            }
        }
        stage('Test') {
            steps {
                // Run Maven Wrapper Commands
                sh "./mvnw test"

                echo 'Testing the Project with Maven Wrapper test'
            }
        }
        stage('Package') {
            steps {
                // Run Maven Wrapper Commands
                sh "./mvnw package"

                echo 'Packaging the Project with Maven Wrapper package'
            }
        }
    }
}
