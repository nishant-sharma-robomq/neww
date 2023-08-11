pipeline {
    agent any
    
    stages {
        stage('Build Docker Image') {
            steps {
                script {
                    def imageName = 'my-custom-image'
                    sh 'ls'
                    def dockerfilePath = '.'
                    
                    // Build the Docker image using Docker CLI
                    sh "docker build -t ${imageName} ."
                }
            }
        }
    }
}
