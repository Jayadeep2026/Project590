pipeline {
    agent any

    stages {
        stage('GIT PULL') {
            steps {
                git branch: "master", url: 'https://github.com/Jayadeep2026/Project590.git'
            }
        }
        stage('TEST') {
            steps {
                sh 'flutter test'
            }
        }
        stage('BUILD') {
            steps {
                sh '''
                  #!/bin/sh
                  flutter build web --wasm
                  '''
            }
        }
    }
}