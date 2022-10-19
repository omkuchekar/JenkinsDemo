pipeline {
    agent any 
        stages {
            stage ('verify branch'){
               steps{
                   "$GIT_BRANCH"
                   "my branch"
            }
            stage ('bash scripting'){
               sh '''#!/bin/bash
               date               
               '''

            }
            
         }
      }
}