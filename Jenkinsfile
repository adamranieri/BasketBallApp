pipeline {
    agent { docker { image 'maven:3.3.3' } }
    stages {
        stage('build') {
            steps {
                sh 'mvn package'                            
            }
        }
        stage('deploy'){
            steps{               
                sh 'cp ./target/BBallApp.war var/lib/docker/volumes/webapps/_data'
            }            
        }
    }
}
