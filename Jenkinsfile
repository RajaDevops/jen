pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building the application...'
                // Add your build commands here, like mvn or npm build
            }
        }
        
        stage('Test') {
            steps {
                echo 'Running unit tests...'
                // Add your test commands here, like mvn test
            }
        }
        
        stage('Integration Test') {
            when {
                branch 'main'
            }
            steps {
                echo 'Running integration tests on main branch...'
                // Add your integration test commands here
            }
        }

        stage('Staging Deployment') {
            steps {
                echo 'Deploying to staging environment...'
                // Add your staging deployment commands
            }
        }
        
        stage('Approval for Production') {
            input {
                message "Deploy to Production?"
                ok "Proceed with deployment"
            }
            steps {
                echo 'Approved for production deployment...'
            }
        }
        
        stage('Production Deployment') {
            when {
                branch 'main'
            }
            steps {
                echo 'Deploying to production environment...'
                // Add your production deployment commands
            }
        }
    }
}
