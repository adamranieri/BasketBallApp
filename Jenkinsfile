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
                sh "cp -f ./target/*.war/ home/ec2-user/RevOpsMaven/apache-tomcat-9.0.20/webapps"  
            }            
        }
    }
}
