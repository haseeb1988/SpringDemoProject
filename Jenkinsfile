pipeline {
    agent any
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
