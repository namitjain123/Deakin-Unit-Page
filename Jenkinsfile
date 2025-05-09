pipeline {
    agent any
    
    stages {
        stage('Install Dependencies') {
            steps {
                script {
                    // Install dependencies using npm
                    sh 'npm install'
                }
            }
        }

        
        stage('Build') {
            steps {
                script {
                    // Build the project using npm (you can use any build tool you prefer)
                    sh 'npm run build'  // This assumes you have a "build" script in package.json
                }
            }
        }
        // stage('Lint') {
        //     steps {
        //         script {
        //             // Run linting (optional, to check code quality)
        //             sh 'npm run lint'  // You can configure linting using ESLint or similar tools
        //         }
        //     }
        // }
        stage('Test') {
            steps {
                script {
                    // Run unit tests (optional, depending on your project)
                    sh 'npm test'  // Assuming you have tests configured in your package.json
                }
            }
        }
        stage('Deploy to Staging') {
            steps {
                script {
                    // Deploy the code to a staging environment (example)
                    sh 'npm run deploy-staging'  // You can configure this to deploy to any server
                }
            }
        }
        stage('Deploy to Production') {
            steps {
                script {
                    // Deploy to the production environment
                    sh 'npm run deploy-production'  // Deploy to production
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
