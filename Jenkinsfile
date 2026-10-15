pipeline {
	agent any

	// environment {
	// 	IMAGE_NAME = 'student-registry-app'
	// }

	stages {
		stage('Install NPM Dependencies') {
			steps {
				bat 'npm install'
			}
		}

		stage('Run Tests') {
			steps {
				bat 'npm test'
			}
		}
	}
}
