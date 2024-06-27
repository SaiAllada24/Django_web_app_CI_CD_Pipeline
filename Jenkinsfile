pipeline {
    agent any
    
    stages {
        stage('Build') {
            steps {
                // Replace with appropriate Windows command
                bat 'python manage.py migrate'
                bat 'python manage.py collectstatic --noinput'
            }
        }
        stage('Test') {
            steps {
                // Replace with appropriate Windows command
                bat 'python manage.py test'
            }
        }
        stage('Deploy') {
            steps {
                // Replace with appropriate Windows command
                bat 'python manage.py runserver'
            }
        }
    }
}
