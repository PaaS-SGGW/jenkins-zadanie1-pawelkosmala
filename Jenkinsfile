pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'echo "Hello World"'
                script {
                    docker.withServer('tcp://192.168.0.22:2375') {
                        echo 'Inside with Server'
                        sh 'docker info'
                    }
            }
        }
    }
}
