pipeline {
    agent any
    triggers {
    pollSCM('* * * * *') 
    }
    stages {
        stage('Build project') {
            steps {
                bat 'dotnet build'
            }
        }
        stage('Execute tests') {
            steps {
                bat 'dotnet test'
            }
        }
    }
}