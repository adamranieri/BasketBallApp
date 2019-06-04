pipeline {
    stages {
        stage('build') {
            steps {
                sh "mvn package"                           
            }
        } 
        stage('deploy'){
            steps{ 
                sh "echo 'deploying'"  
            }            
        }
    }
}
