pipeline {
    agent {
        docker {
            image 'node:lts-bullseye-slim' 
            args '--user root -v /var/run/docker.sock:/var/run/docker.sock && -p 3000:3000' 
        }
    }
    stages {
        stage('Build') { 
            steps {
                sh 'npm install' 
            }
        }
    }
}