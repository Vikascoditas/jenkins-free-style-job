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
                bat 'python -m pip install Flask'
            }
        }
        
        stage('Run Flask App') {
            steps {
                bat 'python main.py'
            }
        }
    }
}
