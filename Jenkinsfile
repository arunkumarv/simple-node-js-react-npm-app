pipeline {
    agent {
        docker {
            image 'node:6-alpine'
            args '-u root:root -p 3000:3000 --privileged -v /var/run/docker.sock:/var/run/docker.sock'

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