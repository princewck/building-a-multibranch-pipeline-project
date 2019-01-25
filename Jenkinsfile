pipeline {
    agent {
        docker {
            image 'node:6-alpine'
            args '-p 3000:3000'
        }
    }
    stages {
        stage('构建') {
            steps {
                sh 'npm install'
            }
        }
        stage('部署') {
            steps {
                sh 'npm start'
            }
        }
    }
}