pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        echo 'gfg'
      }
    }

    stage('test') {
      steps {
        timeout(time: 30, unit: 'DAYS')
      }
    }

    stage('push') {
      steps {
        retry(count: 3)
      }
    }

  }
}