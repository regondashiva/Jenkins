pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                echo 'Checkout Stage'
            }
        }

        stage('Build') {
            steps {
                bat 'docker ps'
            }
        }

        stage('Test') {
            steps {
                bat 'docker exec MyContainer ls'
            }
        }

        stage('Deploy') {
            steps {
                bat 'docker exec MyContainer apt-get update'
            }
        }

        stage('Verify') {
            steps {
                bat 'docker exec MyContainer vim --version'
            }
        }
    }
}
