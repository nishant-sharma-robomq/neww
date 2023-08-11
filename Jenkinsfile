pipeline {
    agent any
    stages {
        stage('Build Docker Image') {
            steps {
                script {
                    def imageName = 'my-custom-image'
                    def dockerfile = 'Dockerfile'
                    
                    echo "Building Docker image..."
                    docker.build(imageName, "-f ${dockerfile} .")
                    echo "Docker image built: ${imageName}"
                }
            }
        }
    }
}
