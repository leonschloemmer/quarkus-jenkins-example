pipeline {
    agent { docker { image 'quay.io/quarkus/centos-quarkus-maven:19.3.1-java11' } }
    stages {
        stage('build') {
            steps {
                sh 'ls -al'
                sh 'mvn -f pom.xml -Pnative clean package'
            }
        }
    }
}