pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                wsl sh 'ls'
                archiveArtifacts artifacts: '**/target/*.jar', fingerprint: true
            }
        }
    }
}
