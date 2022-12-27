pipeline {
  agent any
  stages {
    stage('Build') {
      parallel {
        stage('Build') {
          steps {
            echo 'This is build stage: 1'
          }
        }

        stage('Build:2') {
          steps {
            echo 'This is build step 2.'
          }
        }

      }
    }

    stage('Test') {
      steps {
        sh 'echo Test'
      }
    }

    stage('Deploy') {
      steps {
        sh 'echo Deploy'
      }
    }

  }
}