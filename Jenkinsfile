pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh '''
                    docker --version
                    docker build -t nginx:v2 .
                    
                '''
            }
        } 
        stage('deploy') {
            steps {
                sh '''
                    docker images
                    docker run -d --name container1 -p 80:80 nginx:v2
                    docker ps
                    
                '''
            }
        }             
    }
}