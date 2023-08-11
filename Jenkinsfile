pipeline {
    agent any

    stages {
        stage('Addition') {
            steps {
                script {
                    def userInput1 = input(
                        message: 'Enter the first number:',
                        parameters: [string(defaultValue: '', description: 'First number', name: 'NUMBER1')]
                    )
                    def userInput2 = input(
                        message: 'Enter the second number:',
                        parameters: [string(defaultValue: '', description: 'Second number', name: 'NUMBER2')]
                    )

                    def number1 = userInput1.toInteger()
                    def number2 = userInput2.toInteger()
                    def sum = number1 + number2

                    echo "The sum of ${number1} and ${number2} is ${sum}"
                }
            }
        }
    }
}
