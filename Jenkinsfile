pipeline {
    agent none
    stages {
        stage('build') {
            agent { docker 'maven:3-alpine' } 
            steps {
                sh "pwd"
                sh "mvn package"                           
            }
        } 
        stage('deploy'){
            steps{               
                sh "pwd"
            }            
        }
    }
}
