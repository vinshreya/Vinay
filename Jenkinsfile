pipeline {
  agent any
  stages {
    stage('Parallel') {
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
            echo 'testing more'            
          }
        }

      }
    }

    stage('Static Code Analysis') {
      steps {
        echo 'SonarQube...'
      }
    }
    stage('deploy') {
      steps {
        echo 'Deploying'
      }
    }

  }
}
