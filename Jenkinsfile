pipeline {
  agent any
  stages {
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
        sh 'magicDeployScript'
      }
    }
  }
}