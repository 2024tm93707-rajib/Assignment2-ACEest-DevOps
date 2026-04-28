pipeline {
    agent any
    stages {
        stage('Clone') {
            steps { git 'https://github.com/your-repo.git' }
        }
        stage('Test') {
            steps { sh 'pytest' }
        }
        stage('Build Docker') {
            steps { sh 'docker build -t aceest:${BUILD_NUMBER} .' }
        }
    }
}
