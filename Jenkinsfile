pipeline {
    agent any
        stages{
            stage('Verify branch'){
                steps{
                    echo "$GIT_BRANCH"
                }
            }
            stage('Docker build'){
                steps{
                   pwsh(script: "docker images -a")
                   pwsh(script :"""
                   cd JenkinsDemo/
                   docker images -a
                   docker build -t jenkine-pipeline .
                   docker images -a
                   cd...
                   """
                   )
                }
            }
        }
}