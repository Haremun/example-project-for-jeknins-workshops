pipeline {
    agent { docker { image 'maven:latest' } }
    stages {
        stage('env info') {
            steps {
				mvn --version
                sh 'java --version'
            }
        }
    }
}
