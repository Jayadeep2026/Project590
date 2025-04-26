pipeline {
    agent any

    stages {
        stage('GIT PULL') {
            steps {
                git branch: "master", url: 'https://github.com/Jayadeep2026/Project590.git'
            }
        }

        stage('BUILD') {
                bat ''' Echo starting build'''
                bat ''' flutter build web --wasm'''
        }
    }
}