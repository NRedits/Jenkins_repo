pipeline {
    agent any

    triggers {
        githubPush() // Trigger the job on GitHub push event
    }

    stages {
        stage('Checkout') {
            steps {
                checkout scm
            }
        }
        stage('Build') {
            steps {
                echo 'Building the project...'
                // Add your build commands here, e.g., compile or package the code
            }
        }
        stage('Test') {
            steps {
                echo 'Running tests...'
                // Add test commands like `mvn test`, `npm test`, etc.
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying the application...'
                // Add deployment steps if necessary
            }
        }
    }
}
