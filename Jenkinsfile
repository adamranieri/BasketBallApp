pipeline {
    agent { docker { image 'maven:3.3.3' } }
    stages {
        stage('build') {
            steps {
                sh "mvn package"                           
            }
        }
        stage('deploy'){
            agent { docker { image 'tomcat:latest' } }
            steps{               
                sh 'catalina --version'
            }            
        }
    }
}
