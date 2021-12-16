pipeline {
    agent any

    stages {
        stage('Checking the docker containers') {
            steps {
                sh 'docker ps'
            }
        }
        stage('Checking all containers') {
            steps {
                sh 'docker ps -a'
            }
        }
        stage('Checking images') {
            steps {
                sh 'docker images ls'
            }
        }

    }
}