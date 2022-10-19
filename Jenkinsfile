pipeline {
    agent any 
        stages {
            stage ('verify branch'){
               steps{
                  echo "$GIT_BRANCH"
                  echo "my branch"
            }
            stage ('bash scripting'){
               sh '''#!/bin/bash
               date               
               '''

            }
            
         }
      }
}