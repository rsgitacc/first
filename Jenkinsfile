//Jenkinsfile (Declarative Pipeline)
pipeline {
    agent any
        stages {
        stage('Build') {
            steps {
                echo 'Building..Executing Maven...'
                git 'https://github.com/rsgitacc/first.git'
                bat '.\mvnw clean compile'
                  
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
