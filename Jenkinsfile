pipeline {
  agent any
  stages {
    stage('Parallel Build') {
      steps {
        parallel(
          "Chromez": {
            sh 'echo \'do real work\''
            
          },
          "Safari": {
            sh 'echo \'do more real work\''
            
          }
        )
      }
    }
    stage('Deploy To Test') {
      steps {
        sh 'breakit'
      }
    }
  }
  environment {
    USER = 'hello'
  }
}