pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                git branch: 'main', url: 'https://github.com/trungvuthanh/simple-python-test-ci.git'
                bat 'python main.py'
                echo 'Building application...'
            }
        }
        
        stage('Test') {
            steps {
                bat 'python main.py'
                echo 'Testing application...'
            }
        }
    }
}
