node {
    checkout scm
    stage('Build') {
        echo "Build"
        docker.build('jenkins-quarkus-quickstart/ci-example')
    }
    stage('Deploy') {
        docker.image('jenkins-quarkus-quickstart/ci-example').withRun('-p 33444:8080') {
            echo "container running wohooo"
        }
    }
}