pipeline {
    agent any
    
    stages {
        stage('Test') {
            steps {
                python --version
                 bat "\"C:\\Users\\Coditas\\AppData\\Local\\Programs\\Python\\Python310\\python.exe\" --version"
            }
        }
        
        stage('Build') {
            steps {
                bat "\"C:\\Users\\Coditas\\AppData\\Local\\Programs\\Python\\Python310\\python.exe\" main.py"
            }
        }
    }
}
