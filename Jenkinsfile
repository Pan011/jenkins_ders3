pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building the project...'
                // Build commands go here
            }
        }

        stage('Deploy to Staging') {
            steps {
                echo 'Deploying to staging environment...'
                // Staging deployment commands go here
            }
        }

        stage('Manual Approval') {
            steps {
                // Kullanıcıdan devam etmek için onay iste
                input message: 'Deploy to Production?', ok: 'Deploy'
            }
        }

        stage('Deploy to Production') {
            steps {
                echo 'Deploying to production environment...'
                // Production deployment commands go here
            }
        }
    }
}
