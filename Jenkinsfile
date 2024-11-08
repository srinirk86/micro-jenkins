pipeline {
    agent any  // Use any available agent for this pipeline

    stages {
        stage('Checkout') {
            steps {
                // Checkout the code from Git repository
                git url: 'https://github.com/srinirk86/micro-jenkins.git', branch: 'main'
            }
        }

        stage('Build') {
            steps {
                // Basic shell command (replace with your actual build commands)
                echo 'Running basic build steps'
                sh 'echo "Building the project..."'
            }
        }

        stage('Test') {
            steps {
                // Run tests or any other basic operations
                echo 'Running tests (example step)'
                sh 'echo "Running tests..."'
            }
        }
    }

    post {
        success {
            echo 'Build was successful!'
        }
        failure {
            echo 'Build failed.'
        }
    }
}
