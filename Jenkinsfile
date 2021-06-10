pipeline {
    agent any
    stages {
        stage('test') {
            steps {
                git branch: 'main', url: 'https://github.com/trungvuthanh/simple-python-test-ci.git'
                sh "pip install poetry"
                sh "poetry install"
                sh "poetry run pytest"
                echo 'testing application...'
            }
        }
    }
}
