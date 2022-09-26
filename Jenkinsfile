pipeline {
    agent any
        stages{
            stage('HellVerify branch'){
                steps{
                    echo $GIT_BRANCH
                }
            }
            stage('Hello from bash script'){
                steps{
                   sh 'echo \'Hello from shell script\''
                }
            }
        }
}