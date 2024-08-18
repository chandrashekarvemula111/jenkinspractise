pipeline {
    agent none
    stages {
        stage ('AWS') {
            agent {
                docker { image 'amazon/aws-cli:latest' }
                steps {
                    sh '''
                        aws --version
                    '''
                }
            }
        }
    }
}
