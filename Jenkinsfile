pipeline {
    agent any 
    environment {
        PATH="/usr/local/maven/bin:$PATH"
    }
    stages {
        stage('GIT CHECKOUT') {
            steps {
                git 'https://github.com/aja6009/pipecode'
            }
        }
        stage('MAVEN BUILD') {
            steps {
                sh "mvn clean package"
            }
        }
    }
}
