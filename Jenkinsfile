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
                sh 'docker run -it -d -p 80:8080 -v $(pwd)/target/*.war:/usr/local/tomcat/webapps/bball.war tomcat'
            }            
        }
    }
}