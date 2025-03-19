pipeline {
    agent any 
    stages {
        stage('Build') {
            steps {
                sh 'g++ -o my_program pipeline.cpp' 
                echo 'Build Stage Successful'
            }
        }
        stage('Test') {
            steps {
                sh 'hello' 
                echo 'Test Stage Successful'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deployment Successful'
            }
        }
    }
    post {
        failure {
            echo 'Pipeline failed'
        }
    }
}
