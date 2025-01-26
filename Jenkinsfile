pipeline {
  agent any
  stages {
    stage('Verify Environment') {
      steps {
        script {
          sh 'echo $PATH'
          sh 'which node'
          sh 'node -v'
        }
      }
    }
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
