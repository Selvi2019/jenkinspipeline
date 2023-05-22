pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'I want to build'
      }
    }

    stage('Test') {
      parallel {
        stage('Test') {
          steps {
            echo 'TEsting'
          }
        }

        stage('Deploy') {
          steps {
            echo 'DEploy'
          }
        }

      }
    }

  }
}