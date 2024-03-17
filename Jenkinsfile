pipeline {
    agent any

    environment {
        // Kimlik bilgilerini ortam değişkenlerine atayarak kullanın
        MY_SECRET = credentials('github-token')
    }

    stages {
        stage('Checkout') {
            steps {
                echo 'Checking out code...'
                // Checkout commands go here
            }
        }

        stage('Build') {
            steps {
                echo 'Building...'
                // Build commands go here
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying...'
                sh '''
                # Use the credentials securely
                echo "Deploying using ${MY_SECRET} user"
                # Insert deployment commands here
                # For example, using credentials to authenticate against a server
                '''
            }
        }
    }
}
