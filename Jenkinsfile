pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                git branch: 'main', url: 'https://github.com/trungvuthanh/simple-python-test-ci.git'
            }
        }
        
        stage('Test') {
            steps {
                bat 'pytest -v -s'
                echo 'Testing application...'
            }
        }
    }
}
