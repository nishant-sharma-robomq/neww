pipeline {
    agent any
    
    stages {
        stage('Add Numbers') {
            steps {
                script {
                    def num1 = 5
                    def num2 = 7
                    def sum = num1 + num2
                    echo "Sum of ${num1} and ${num2} is ${sum}"
                }
            }
        }
    }
}
