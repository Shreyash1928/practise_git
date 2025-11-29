pipeline {
    agent any

    options {
        timestamps()
    }
    wrappers {
        ansiColor('xterm')
    }

    stages {
        stage('Clone Repository') {
            steps {
                git branch: 'main',
                    url: 'https://github.com/Shreyash1928/practise_git'
            }
        }

        
    }

    post {
        success {
            echo "Build completed successfully!"
        }
        failure {
            echo "Build failed!"
        }
    }
}