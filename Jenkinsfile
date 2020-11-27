pipeline {
  agent any
  stages {
    stage('cc') {
      steps {
        sh 'echo "aa"'
        input(message: 'are you ok', id: 'admin', ok: 'yes', submitter: 'admin')
      }
    }

  }
}