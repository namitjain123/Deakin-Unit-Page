pipeline {
    agent any

    stages {
        stage('Install Dependencies') {
            steps {
                script {
                    // Install dependencies using npm
                    echo "Using npm to install project dependencies"
              
                }
            }
        }

        stage('Build') {
            steps {
                script {
                    // Build the project using npm
                    echo "Using npm to build the project (build tool)"
               
                }
            }
        }

        stage('Lint') {
            steps {
                script {
                    // Run linting (optional, to check code quality)
                    echo "Using ESLint to check the code for issues and maintain quality"
                
                }
            }
        }

        stage('Test') {
            steps {
                script {
                    // Run unit tests (optional, depending on your project)
                    echo "Using Jest for unit testing"
                 
                }
            }
        }

        stage('Deploy to Staging') {
            steps {
                script {
                    // Deploy the code to a staging environment (example)
                    echo "Using npm to deploy to a staging environment"
               
                }
            }
        }

        stage('Deploy to Production') {
            steps {
                script {
                    // Deploy to the production environment
                    echo "Using npm to deploy to production"
              
                }
            }
        }
    }

    post {
        always {
            // Cleanup or notifications
            echo 'Pipeline finished!'
        }
    }
}
