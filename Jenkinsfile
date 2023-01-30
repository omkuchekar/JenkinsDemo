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
                              cd azure-vote/
                              docker build -t jenkine-pipelines .
                              docker images -a
                        '''
               }
            }
        }
}
