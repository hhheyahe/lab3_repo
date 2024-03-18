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

        stage('Build JavaScript') {
            steps {
                sh 'npm install'  // Install dependencies (if any)
                sh 'npm run build'  // Execute the build command or script
            }
        }

        stage('Archive File') {
            steps {
                archiveArtifacts artifacts: 'lab3task7.js', fingerprint: true
            }
        }
    }
}
