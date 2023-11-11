pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                wsl
                sh 'make'
                archiveArtifacts artifacts: '**/target/*.jar', fingerprint: true
            }
        }
    }
}
