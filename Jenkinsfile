pipeline{
    agent {label 'Jenkins-Agent'}
    tools{
        jdk 'java17'
        maven 'Maven3'
    }
    stages{
        stage("Cleanup Workspace"){
            steps{
                cleanWs()
            }
        }
        stage("Git Checkout"){
            steps{
                git branch: 'main', credentialsId: 'github', url: 'https://github.com/shubhamlole/registration-app.git'
            }
        }
    }
}
