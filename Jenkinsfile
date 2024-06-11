pipeline {
	agent any

	stages {
		stage('Checkout') {
			steps {
				checkout scm
			}
		}
		stage('Client Tests') {
			steps {
				dir('client') {
					bat 'npm install'
					bat 'npm test'
				}
			}
		}
	}

}
