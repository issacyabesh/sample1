pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                checkout scmGit(branches: [[name: '*/master']], extensions: [], userRemoteConfigs: [[credentialsId: '786e9e09-c306-4f2e-aef6-98a1e7a82f52', url: 'https://github.com/issacyabesh/sample1.git']])
            }
        }
        stage('test') {
            steps {
                sh 'python3 test.py'
            }
        }
        stage('test2') {
            steps {
                sh 'python3 test2.py'
            }
        }
    }
}
