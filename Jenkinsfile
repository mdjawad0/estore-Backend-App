pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                // Get some code from a GitHub repository
                git 'https://github.com/mdjawad0/estore-Backend-App.git'

                // Run Maven Commands
                sh "mvn compile"

                echo 'Building the Project with Maven compile'
            }
        }
        stage('Test') {
            steps {
                // Run Maven Commands
                sh "mvn test"

                echo 'Testing the Project with Maven test'
            }
        }
        stage('Package') {
            steps {
                // Run Maven Commands
                sh "mvn package"

                echo 'Packaging the Project with Maven package'
            }
        }
    }
}
