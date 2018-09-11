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
        sh 'npm run cy:verify'
        sh 'npm run cy:run'
      }
    }
  }
}
