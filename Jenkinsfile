pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building the project...'
                // Build commands go here
            }
        }

        stage('Test') {
            steps {
                echo 'Testing the project...'
                // Test commands go here

            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying the project...'
                // Deploy commands go here
            }
        }
    }

    post {
        success {
            echo 'Pipeline completed successfully!'
            // Başarılı olduğunda yapılacak işlemler (örneğin, bildirim gönderme)
        }

        failure {
            echo 'Pipeline failed!'
            // Hata olduğunda yapılacak işlemler (örneğin, hata analizi)
        }

        always {
            echo 'This will always run regardless of the result.'
            // Her durumda yapılacak işlemler (örneğin, temizleme işlemleri)
        }
    }
}