pipeline {
    agent any

    tools {
        // Jenkins yapılandırmasında tanımlı Maven sürümünü kullan
        maven 'maven-3.9.6'
    }

    stages {
        stage('Checkout') {
            steps {
                echo 'Checking out source code...'
                // Source code checkout steps
            }
        }

        stage('Build') {
            steps {
                echo 'Building with Maven'
                // Maven ile proje inşa et
                sh 'mvn clean install'
            }
        }

        stage('Test') {
            steps {
                echo 'Running tests'
                // Maven ile test çalıştır
                sh 'mvn test'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying application'
                // Maven ile deploy işlemi
                sh 'mvn deploy'
            }
        }
    }
}