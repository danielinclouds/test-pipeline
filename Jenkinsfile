pipeline {
    agent { docker { image 'ubuntu:latest' } }
    stages {
        stage('hello_world') {
            steps {
                sh 'echo Hello World'
            }
        }
    }
}
