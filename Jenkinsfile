pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                bat 'make'
                archiveArtifacts artifacts: '**/target/*.jar', fingerprint: true
            }
        }
    }
}
