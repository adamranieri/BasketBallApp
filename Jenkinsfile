pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                sh "mvn package"                           
            }
        } 
        stage('deploy'){
            steps{ 
                sh "pwd"
                sh "echo 'deploying'"  
            }            
        }
    }
}
