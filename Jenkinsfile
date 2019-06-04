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
                sh "cp -f ./target/BBallApp.war /home/ec2-user/RevOps/apache-tomcat-9.0.20/webapps"  
            }            
        }
    }
}
