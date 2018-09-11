pipeline {
  agent {
    docker {
      image 'cypress/base:10'
    }
  }

  stages {

    stage('cypress - test') {



      // environment {
      //   // TERM 'xterm'
      // }

      steps {
        sh 'npm ci'
        // sh '$(npm bin)/cypress run --record --key <record_key>'
      }
    }
  }
}
