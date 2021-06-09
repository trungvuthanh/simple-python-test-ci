pipeline {
    
    agent any

    stages {

        stage('test') {

            steps {
                sh 'pytest -v -s'
                echo 'testing application...'
            }
        }
    }
}
