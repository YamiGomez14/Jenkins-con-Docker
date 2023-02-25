#!/usr/bin/env groovy
pipeline {
    agent {
    docker {
        image 'docker:latest'
        args '-v /var/run/docker.sock:/var/run/docker.sock'
    }
}
    stages {
        stage('Stage 1'){
            steps{
                echo "Prueba 2"
            }
        }
        stage('Docker Compose Build') {
            steps {
                sh 'docker-compose build'
            }
        }

        stage('Docker Compose Up') {
            steps {
                sh 'docker-compose up -d'
            }
        }
    
    }
}
