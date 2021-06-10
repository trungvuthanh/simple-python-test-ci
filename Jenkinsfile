pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                git branch: 'main', url: 'https://github.com/trungvuthanh/simple-python-test-ci.git'
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
