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
                sh 'docker image ls'
            }
        }
        stage('Building the docker image') {
            steps {
                cd 'cd $FOLDER_PATH'
                sh 'docker build -t python-app2'
            }
        }
        stage('Running the docker container') {
            steps {
                sh 'docker run python-app2'
            }
        }
    }
}