pipeline {
  agent any
  stages {
    stage('compilation') {
      parallel {
        stage('compilation') {
          steps {
            echo 'Compiling'
            echo 'Continue Compiling'
          }
        }

        stage('test') {
          steps {
            echo 'testing'
          }
        }

      }
    }

    stage('deploy') {
      steps {
        echo 'Deploying'
      }
    }

  }
}