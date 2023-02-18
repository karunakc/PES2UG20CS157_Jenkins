pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'g++ -o PES2UG20CS157-1 hello.cpp'
                echo 'Build success'
            }
        }
        stage('Test') {
            steps {
                sh './/PES2UG20CS157-1'
                echo 'Test success'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploy success'
            }
        }
    }
    post {
        failure {
            echo 'Pipeline failed'
        }
    }
}
