pipeline{
    agent {label 'Jenkins-Agent'}
    tools{
        jdk 'java17'
        maven 'Maven3'
    }
    stages{
        stage("Cleanup Workspace"){
            step{
                cleanWs()
            }
        }
        stage("Git Checkout"){
            step{
                git branch: 'main', credentialsId: 'github', url: 'https://github.com/shubhamlole/registration-app.git'
            }
        }
    }
}
