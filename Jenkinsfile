pipeline {
    agent { docker { image 'maven:3.3.3' } }
    stages {
        stage('build') {
            steps {
                sh "mvn package"                           
            }
        }
        stage('deploy'){
            steps{               
                sh "docker ps"
            }            
        }
    }
}
