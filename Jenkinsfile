pipeline {
  agent any
  stages {
    stage('dev') {
      parallel {
        stage('dev') {
          steps {
            echo 'hi'
            sleep 10
          }
        }

        stage('build') {
          steps {
            build 'test'
          }
        }

      }
    }

    stage('QA') {
      steps {
        echo 'welcome'
      }
    }

  }
}