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

    stage('error') {
      steps {
        echo 'test'
        timeout(unit: 'MINUTES', time: 30) {
          sh 'echo'
        }

        sleep 3
      }
    }

  }
}