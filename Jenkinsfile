pipeline {
    agent { docker { image 'maven:3.6.3' } }
    stages {
        stage('build') {
            steps {
                sh 'ls -al'
                sh 'mvn -f pom.xml -Pnative clean package'
            }
        }
    }
}