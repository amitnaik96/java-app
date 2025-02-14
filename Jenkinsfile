pipeline {
    agent any

    stages {
        stage('Clone Repository') {
            steps {
                git 'https://github.com/amitnaik96/java-app.git'
            }
        }
        stage('Build and Run') {
            steps {
                bat 'javac src/Main.java -d out'
                bat 'java -cp out Main'
            }
        }
    }
}
