pipeline {
    agent {
        docker.withServer('tcp://swarm.example.com:2375') { image 'centos:7' }
    }
    stages {
        stage('Build') {
            steps {
                sh 'echo "Hello World"'
                sh '''
                    echo "Multiline shell steps works too"
                    cat /etc/redhat-release
                    ls -lah
                '''
            }
        }
    }
}
