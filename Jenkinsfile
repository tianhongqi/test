pipeline {
  agent any
  stages {
    stage('cc') {
      steps {
        sh 'echo "aa"'
        input(message: 'are you ok', id: 'admin', ok: 'yes', submitter: 'admin')
      }
    }

    stage('dd') {
      steps {
        echo 'ea'
        retry(count: 1) {
          sleep 1
        }

        ws(dir: '/home/jenkins') {
          junit 'de'
        }

      }
    }

  }
}