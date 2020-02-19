pipeline {
    agent { docker { image 'docker:19' } }
    stages {
        stage('build') {
            steps {
                sh 'ls -al'
                sh 'sudo docker build -f src/main/docker/Dockerfile.multistage -t jenkins-quickstart/ci-example .'
            }
        }
    }
}