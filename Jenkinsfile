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
                sh "cd ./target"
                sh "cp -f *'.war' /home/ec2-user/RevOpsMaven/apache-tomcat-9.0.20/webapps"  
            }            
        }
    }
}
