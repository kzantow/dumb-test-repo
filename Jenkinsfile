pipeline {
  agent any
  stages {
    stage('Parallel Build') {
      steps {
        parallel(
          "error": {
            sh 'echo \'do real workz\''
            
          },
          "Safari": {
            sh 'echo \'do more real work\''
            
          }
        )
      }
    }
    stage('Deploy To Test') {
      steps {
        sh '''# fix it
echo woorrd'''
      }
    }
  }
  environment {
    USER = 'hello'
  }
}