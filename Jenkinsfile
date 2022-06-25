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
                script {
                    sh 'npm install' 
                }
            }
        }
    }
}