pipeline {
    agent any

    stages {

        stage('Clone') {
            steps {
                git branch: 'main', url: 'https://github.com/01Amirkhan/Online-ticket.git'
            }
        }

        stage('Install') {
            steps {
                sh 'echo Installing Dependencies'
            }
        }

        stage('Build Docker') {
            steps {
                sh 'docker build -t online-ticket .'
            }
        }
    }
}
