pipeline {
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
                sh "ssh 100.26.245.193 "
                sh "pwd"
            }            
        }
    }
}
