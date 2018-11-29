pipeline {
    agent { docker { image 'maven:3.3.3' } }
    stages {
        stage('hello_world') {
            steps {
                sh 'echo Hello World'
            }
        }
    }
}
