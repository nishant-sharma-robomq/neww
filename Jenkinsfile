pipeline {
    agent any

    stages {
        stage('Addition') {
            steps {
                script {
                    def userInput1 = ${NUMBER1}
                    def userInput2 = ${NUMBER2}

                    def number1 = userInput1.toInteger()
                    def number2 = userInput2.toInteger()
                    def sum = number1 + number2

                    echo "The sum of ${number1} and ${number2} is ${sum}"
                }
            }
        }
    }
}
