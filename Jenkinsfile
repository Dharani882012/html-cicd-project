pipeline {
    agent any

    stages {
        stage('Build Image') {
            steps {
                bat 'docker build -t web-app .'
            }
        }

        stage('Run Container') {
            steps {
                bat 'docker run -d -p 8081:80 web-app'
            }
        }
    }
}
