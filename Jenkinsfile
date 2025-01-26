pipeline {
  agent any
  environment {
    PATH = "/usr/local/bin:$PATH"  // Adjust this to where node is located on your server
  }
  stages {
    stage('Build') {
      steps {
        nodejs('Node') {
          echo 'Building Application.....'
          sh 'npm install'
        }
      }
    }
  }
}
