pipeline {
    agent { docker { image 'python:3.5.1' } }
    stages {
        stage('build') {
            steps {
                sh 'python --version'
                sh 'pytest'
                sh 'cd cpp_testing && make'
            }
        }
    }
}
