pipeline {
  agent any
  stages {
    stage('checkout') {
      steps {
        sleep 1
      }
    }

    stage('build') {
      steps {
        echo 'atest'
      }
    }

    stage('deploy') {
      parallel {
        stage('deploy') {
          steps {
            sh 'echo'
            sh 'echo'
            slackSend()
          }
        }

        stage('deploy3') {
          steps {
            echo 'test'
          }
        }

        stage('deploy2') {
          steps {
            echo 'test'
          }
        }

      }
    }

    stage('') {
      steps {
        echo 'test'
      }
    }

  }
}