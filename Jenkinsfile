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
                  sh 'ls -la'
                  sh 'npm install'
                  sh 'npm run build'
              }
            }
        
        stage('Archive File') {
            steps {
                archiveArtifacts artifacts: 'lab3task7.js', fingerprint: true
            }
        }

    }
}
