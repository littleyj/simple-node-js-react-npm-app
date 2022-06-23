pipeline {
    agent {
        docker {
            image 'node:14.16-alpine'
            args '-p 3000:3000' 
        }
    }
    stages {
        stage('Build') { 
            steps {
                echo 'this works'
                sh 'echo "Hello World!"'
                sh '''python --version'''
                sh 'npm install' 
            }
        }
    }
}