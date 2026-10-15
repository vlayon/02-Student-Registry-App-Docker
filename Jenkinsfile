pipeline {
    agent any

    stages {
        stage('Install NPM Dependencies') {
            steps {
                bat 'npm install'
            }
        }

        stage('Run Tests in Parallel') {
            parallel {
                stage('Test Suite 1') {
                    steps {
                        bat 'npm test'
                    }
                }
                stage('Test Suite 2') {
                    steps {
                        echo 'run tests in parallel'
                    }
                }
            }
        }
    }
}
