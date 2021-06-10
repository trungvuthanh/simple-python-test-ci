pipeline {
    agent { docker { image 'python:3.8.5' } }
    stages {
        stage('build') {
            steps {
                sh 'python main.py'
                echo 'building application...'
            }
        }
        
        stage('test') {
            steps {
                sh 'pytest -v -s'
                echo 'testing application...'
            }
        }
    }
}
