pipeline {
    agent any
    environment {
    PATH = "/opt/apache-naven-3.9.6/bin: $PATH"
    stages {
stage('Checkout') {
            steps {
                checkout scmGit(branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[url: 'https://github.com/haseeb1988/SpringDemoProject']])
            }
        }
        stage('Build') {
            steps {
                 sh 'mvn clean install'


            }
        }
    }
}
