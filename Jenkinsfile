pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Build Compiled'
      }
    }

    stage('Test1') {
      parallel {
        stage('Test1') {
          steps {
            echo 'Test compiled 1'
          }
        }

        stage('Test 2') {
          steps {
            echo 'Test Compiled 2'
          }
        }

      }
    }

    stage('Deply') {
      steps {
        echo 'Deploy Complrted'
      }
    }

  }
}