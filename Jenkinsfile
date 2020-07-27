pipeline {
    agent {
    label 'docker' 
  }
  stages {
      stage('Docker Node'){
       agent {
        docker {
            label 'docker' 
            image 'node:6-alpine' 
            args '-p 3000:3000' 
        }
    }
      }
        stage('Build') { 
            steps {
                sh 'npm install' 
            }
        }
    }
}
