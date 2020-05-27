pipeline {
    agent { docker { image 'maven:latest' } }
    stages {
        stage('env info') {
            steps {
				sh 'mvn --version'
                sh 'java --version'
            }
        }
    }
}
