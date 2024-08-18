pipeline {
    agent any

    stages {
        stage ('connect') {
            agent 
                docker {
                    image 'amazon/aws-cli:latest'
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