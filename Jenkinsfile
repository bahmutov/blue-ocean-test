pipeline {
  stages {

    stage('cypress - test') {

      agent {
        docker {
          image 'cypress/base:10'
        }
      }

      environment {
        TERM 'xterm'
      }

      steps {
        sh 'npm ci'
        // sh '$(npm bin)/cypress run --record --key <record_key>'
      }
    }
  }
}
