pipeline {
    agent any

    stages {
        stage ('AWS') {
            agent {
                docker {
                image 'amazon/aws-cli:latest'
            }

            }
        }
        stage('Build') {
            steps {
                sh '''
                    aws --version
                '''
            }
        }           
    }
}