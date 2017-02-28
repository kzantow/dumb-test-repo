pipeline {
  agent any
  stages {
    stage('Pre-Build') {
      steps {
        sh 'echo "woot"'
      }
    }
    stage('Parallel Build') {
      steps {
        parallel(
          "Chrome": {
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
        sh 'echo this one works'
      }
    }
  }
}