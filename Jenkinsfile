pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                // Get some code from a GitHub repository
                git 'https://github.com/mdjawad0/estore-Backend-App.git'

                // Run Maven Wrapper Commands
                sh "sudo ./mvnw compile -S"

                echo 'Building the Project with maven compile'
            }
        }
        stage('Test') {
            steps {

                // Run Maven Wrapper Commands
                sh "sudo ./mvnw test -S"

                echo 'Testing the Project with maven test'
            }
        }
        stage('Package') {
            steps {

                // Run Maven Wrapper Commands
                sh "sudo ./mvnw package -S"

                echo 'Packaging the Project with maven package'
            }
        }
    }
}
