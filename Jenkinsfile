pipeline {
    agent any
    stages {
        stage ('Build Docker Image') {
            steps {
                script {
                    dockerapp = docker.build('caco21/kube_news:${env.BUILD_ID}', '-f ./src/Dockerfile ./src')
                }
            }
        }
    }
}
