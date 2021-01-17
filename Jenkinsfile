pipeline {
    agent any 
    stages {
        stage('git') { 
            steps {
               git credentialsId: 'a7fcf27b-4a62-448e-89e2-4895f6f0ef14', url: 'https://github.com/divyas5/JavaPrograms.git'
               bat 'git.bat'
          
            }
        }
    }
}
