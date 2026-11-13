
pipeline {
    agent any

    tools {
        maven 'Maven'
        jdk 'JDK25'
    }

    stages {
        stage('Checkout') {
            steps {
                git branch: 'main',
                    url: 'https://github.com/PUNEETRA1/MavenDemo3.git',
                    credentialsId: 'github-token'
            }
        }

        stage('Build') {
            steps {
                bat 'mvn clean compile'
            }
        }
    }
}
