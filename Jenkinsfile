pipeline {
  agent any
  stages {
    stage('echo') {
      steps {
        echo 'hello from the trigger'
      }
    }

    stage('echo-again') {
      steps {
        sh '"hello world"'
      }
    }

  }
  triggers {
    cron('H/15 * * * *')
  }
}