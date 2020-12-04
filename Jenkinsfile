pipeline {
    agent any
    tools {
        jdk 'jdk8'
        maven "mvn363"
    }
    stages {
        stage('GIT') {
            steps {
                git 'https://github.com/thiefik/jenkins-workshop1.git'
            }
        }
       
        stage("MVN"){
           steps{
                sh "mvn clean verify"      

            }
        }
    }
}
