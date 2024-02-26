pipeline {
    agent any

    stages {
        stage('SCM Checkout') {
            steps {
                git 'https://github.com/gruntwork-io/terratest.git'
            }
        }
    }
        stage('Build Docker Image') {
            steps {
                script {
                    docker.build('terratest:latest')
                }
            }
        }
}
