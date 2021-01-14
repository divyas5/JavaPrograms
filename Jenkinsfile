pipeline {
    agent none 
    stages {
        stage('Build') { 
            agent {
                docker {
                    image 'python:2-alpine' 
                }
            }
            steps {
                sh 'python -m hello.py' 
                stash(name: 'compiled-results', includes: '/*.py*') 
            }
        }
    }
}
