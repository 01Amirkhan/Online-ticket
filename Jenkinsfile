pipeline {

    agent any

    stages {

        stage('Clone') {
            steps {
                git branch: 'main',
                git 'https://github.com/01Amirkhan/Online-ticket.git'
            }
        }

        stage('Install') {
            steps {
                sh 'npm install'
            }
        }

        stage('Build Docker') {
            steps {
                sh 'docker build -t online-ticket .'
            }
        }
    }
}
