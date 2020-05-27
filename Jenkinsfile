pipeline {
    agent { docker { image 'maven:latest' } }
    stages {
        stage('env info') {
            steps {
                sh 'java --version'
            }
        }
    }
}
