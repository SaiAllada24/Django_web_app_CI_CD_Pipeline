pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'echo "Building the application"'
                sh './gradlew build'
            }
        }
        stage('Test') {
            steps {
                sh 'echo "Running tests"'
                sh './gradlew test'
            }
        }
        stage('Deploy') {
            steps {
                sh 'echo "Deploying application"'
                sh './deploy.sh'
            }
        }
    }
}
