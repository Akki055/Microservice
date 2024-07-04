pipeline {
    agent any

    stages {
        stage('Build & Tag Docker Image') {
            steps {
                script {
                     sh "docker build -t akki058/adservice:latest ."
                    }
                }
            }
        }
        
        stage('Push Docker Image') {
            steps {
                script {
                    sh "docker push akki058/adservice:latest "
                    }
                }
            }
        }
    }
}
