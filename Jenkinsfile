pipeline {
  agent any
  stages {
    stage('dev') {
      steps {
        echo 'this is development stage'
      }
    }

    stage('test') {
      parallel {
        stage('test') {
          steps {
            echo 'This is test stage'
          }
        }

        stage('buid') {
          steps {
            echo 'this is buid'
          }
        }

        stage('deploy') {
          steps {
            echo 'deployment'
          }
        }

        stage('operate') {
          steps {
            echo 'this is operate'
          }
        }

      }
    }

  }
}