pipeline {
    agent any

    stages {
        stage ('AWS') {
            agent {
                docker {
                    image 'amazon/aws-cli'
                    args "--entrypoint=''"
                    reuseNode true
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