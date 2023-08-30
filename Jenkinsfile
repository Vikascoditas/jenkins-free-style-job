pipeline {
    agent any
    
    stages {
        stage('Checkout') {
            steps {
                checkout scm
            }
        }
        
        stage('Install Flask') {
            steps {
                bat 'pip install Flask'
            }
        }
        
        stage('Run Flask App') {
            steps {
                bat 'python main.py'
            }
        }
    }
    
    post {
        always {
            slackSend color: 'good', message: "Flask App Build Successful"
        }
    }
}
