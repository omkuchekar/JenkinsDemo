pipeline {   
    agent any
        stages{
            stage('Verify branch'){
                steps{
                    echo "$GIT_BRANCH"
                }
            }
            stage('Docker build using bash script') {
                steps {
                        sh '''#!/bin/bash
                              docker images -a
                              cd https://github.com/omkuchekar/JenkinsDemo/
                              docker build -t jenkine-pipeline .
                              docker images -a
                              cd...
                        '''
               }
            }
        }
}