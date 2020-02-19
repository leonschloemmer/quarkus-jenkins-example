pipeline {
    agent { docker { image 'ubuntu:bionic' } }
    stages {
        stage('build') {
            steps {
                sh 'ls -al'
                sh 'docker build -f src/main/docker/Dockerfile.multistage -t jenkins-quickstart/ci-example .'
            }
        }
    }
}