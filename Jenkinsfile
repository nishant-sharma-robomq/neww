pipeline {
    agent any

    parameters {
        string(name: 'NUMBER1', defaultValue: '', description: 'Enter the first number')
        string(name: 'NUMBER2', defaultValue: '', description: 'Enter the second number')
    }

    stages {
        stage('Addition') {
            steps {
                script {
                    def number1 = NUMBER1.toInteger()
                    def number2 = NUMBER2.toInteger()
                    def sum = number1 + number2

                    echo "The sum of ${number1} and ${number2} is ${sum}"

                    // Store the sum in a file
                    writeFile file: "apps/sum.txt", text: "${sum}"
                }
            }
        }

        stage('Creating Directory') {
            steps {
                script {
                    // Create the directory if it doesn't exist
                    sh "pwd"
                    sh "ls"
                    sh "mkdir -p apps"
                }
            }
        }

        stage('Creating File and Storing Data') {
            steps {
                script {
                    // Create an empty file named abc.txt
                    writeFile file: "apps/abc.txt", text: "hello, The sum of number is ${sum}"
                }
            }
        }

        stage('Priniting file data') {
            steps {
                script {
                    // Printing file data
                    
                }
            }
        }
    }
}
