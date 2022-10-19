//SCRIPTED

//DECLARATIVE
pipeline {
    //agent any
    agent { docker { image 'node:13.8'}}
    stages {
        stage('Build') {
            steps {
                sh "NOVE --version"
                echo "Build"
            }
        }
        stage('Test') {
            steps {
                echo "Test"
            }
        }
        stage('Integration Test') {
            steps {
                echo "Integration Test"
            }
        }
    } 
    post {
        always {
            echo 'Im awesome'
        }
        success {
            echo 'I run when you are successful'
        }
        failure {
            echo 'I run when you fail'
        }
    }
}
