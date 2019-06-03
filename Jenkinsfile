pipeline {
    agent none
    stages {
        stage('build') {
            agent { docker 'maven:3-alpine' } 
            steps {
                sh "mvn package"                           
            }
        } 
        stage('deploy'){
            agent { docker  'tomcat:latest'  }
            steps{               
                sh 'catalina --version'
            }            
        }
    }
}
