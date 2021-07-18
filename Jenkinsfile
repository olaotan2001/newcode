pipeline {
    agent any
    triggers {
        pollSCM '* * * * *'
    }
    tools {
        maven 'maven'
    }
    stages {
        stage('build'){
            steps{
            sh 'mvn clean'
            sh 'mvn install'
            sh 'mvn package'
                
            }
        }

    }
}
