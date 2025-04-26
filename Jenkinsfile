pipeline {
    environment {

        PATH = "C:\\WINDOWS\\SYSTEM32"

    }

    stages {
        stage('GIT PULL') {
            steps {
                git branch: "master", url: 'https://github.com/Jayadeep2026/Project590.git'
            }
        }

        stage('BUILD') {
            steps {
                bat ''' Echo starting build'''
                bat ''' flutter build web --wasm'''
            }
        }
    }
}