pipeline {
  agent any
  stages {
    stage('Pre-Build') {
      steps {
        sh(script: 'echo "woot"')
      }
    }
    stage('Parallel Build') {
      steps {
        parallel(
          Chrome: {
            sh(script: 'echo \'do real work\'')
          },
          Safari: {
            sh(script: 'echo \'do more real work\'')
            
          }
        )
      }
    }
    stage('Deploy To Test') {
      steps {
        sh(script: 'echo this one works')
      }
    }
  }
}
