//Jenkinsfile (Declarative Pipeline)
pipeline {
    agent any
    tools { maven 'Maven'
        }

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
                echo 'Executing Gradle...'
                withGradle() {
                sh '.gradlew -v'               
                 }
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
