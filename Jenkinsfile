pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Build done successfully'
      }
    }

    stage('DEV') {
      parallel {
        stage('DEV') {
          steps {
            echo 'DEV done'
          }
        }

        stage('QA') {
          steps {
            echo 'QA done'
          }
        }

      }
    }

    stage('prod') {
      steps {
        echo 'prod deployed'
      }
    }

  }
}