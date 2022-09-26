pipeline {
    agent any
        stages{
            stage('Hello'){
                steps{
                    echo 'hello'
                }
            }
            stage('Bye'){
                steps{
                    echo 'Bye'
                }
            }
            stage('Hello from bash script'){
                steps{
                   sh 'echo \'Hello from shell script\''
                }
            }
        }
}