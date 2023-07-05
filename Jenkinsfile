pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
              checkout scmGit(branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[credentialsId: 'e985edd7-67a2-4153-97aa-8c2c4e52f7ae', url: 'https://github.com/Bounzeback/wednesday5thpipeline.git']])
            }
        }
        stage('Test') {
            steps {
                sh 'df -h'
                sh 'touch team6'
            }
        }
        stage(backup){
            steps{
                sh 'pwd'
                sh 'du -h'
            }
        }
    }
}
