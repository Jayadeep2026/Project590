pipeline {
    agent any
    environment {
        PATH = 'C:\\WINDOWS\\SYSTEM32"\\'

            }

    stages {
        stage('GIT PULL') {
            steps {
            withEnv(['PATH+EXTRA=C:\\Program Files\\Git\\bin\\git.exe']){
                git branch: "master",
                url: 'https://github.com/Jayadeep2026/Project590.git'
            }
            }
        }

        stage('BUILD') {
            steps {
            withEnv(['PATH+EXTRA=C:\\Project\\flutter_windows_2.10.5-stable\\flutter\\bin']){
                bat ''' Echo starting build'''
                bat ''' flutter build web --wasm'''
            }
            }
        }
    }
}