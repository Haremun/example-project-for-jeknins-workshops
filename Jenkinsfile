pipeline {
    agent { docker { image 'maven:latest' } }
    stages {
        stage('env info') {
            steps {
				sh 'mvn --version'
                sh 'java --version'
            }
        }
		stage('build'){
			steps {
				sh 'mvn compile'
				sh 'mvn package'
			}
		}
		stage('sleep'){
			steps{
				sleep(time: 1, unit: 'MINUTES')
				echo('Welcome to the secret cow level')
			}
		}
    }
}
