pipeline {
    
    agent {
        
        node {
            label 'my-label'
        }
    }

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
