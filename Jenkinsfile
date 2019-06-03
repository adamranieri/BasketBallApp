pipeline {
    agent { docker { image 'maven:3.3.3' } }
    stages {
        stage('build') {
            steps {
                sh "mvn package"                           
            }
        }
        agent { docker { image 'tomcat:latest' } }
        stage('deploy'){         
            steps{               
                sh 'catalina --version'
            }            
        }
    }
}
