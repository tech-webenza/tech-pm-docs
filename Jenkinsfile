pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building the application...'
                // Example command: sh 'npm install' or sh 'mvn clean compile'
            }
        }
        
        stage('Test') {
            steps {
                echo 'Running tests...'
                // Example command: sh 'npm test' or sh 'mvn test'
            }
        }
        
        stage('Deploy') {
            steps {
                echo 'Deploying application...'
                // Example command: sh './deploy.sh'
            }
        }
    }
    post {
        always {
            echo 'Pipeline finished processing.'
        }
        success {
            echo 'Build and Deployment succeeded!'
        }
        failure {
            echo 'Pipeline failed.'
        }
    }
}
