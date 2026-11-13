pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Starting Maven Build'
                bat 'mvn clean install'
            }
        }
    }
}
