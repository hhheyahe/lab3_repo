pipeline {
    agent any

    stages {
        stage('Hello World') {
            steps {
                sh """
                    echo 'Hello, World!'
                """
            }
        }

        stage('Archive File') {
            steps {
                archiveArtifacts artifacts: 'lab3task7.js', fingerprint: true
            }
        }
    }
}
