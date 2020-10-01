pipeline {
  agent any
  stages {
    stage('echo') {
      steps {
        echo 'hello from Boonchu!'
      }
    }
    stage('echo-again') {
      steps {
        sh '''chmod +x ./testscript.sh
        ./testscript.sh'''
      }
    }
    stage('echo-final') {
      steps {
        echo 'finally, hello to job!'
      }
    }
  }
  triggers {
    cron('H/5 * * * *')
  }
}
