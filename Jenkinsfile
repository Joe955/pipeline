pipeline {
  agent any
  stages {
    stage('Prepare Package') {
      parallel {
        stage('Upload Package') {
          steps {
            sh 'ls'
          }
        }
        stage('Register') {
          steps {
            sleep 15
          }
        }
        stage('Configuration') {
          steps {
            sleep 10
          }
        }
        stage('Check Environment ') {
          steps {
            sleep 10
          }
        }
      }
    }
    stage('SandBox Test') {
      steps {
        echo 'Running SandBox Testing'
      }
    }
    stage('Deploy') {
      steps {
        sleep 5
      }
    }
    stage('A/B Test') {
      steps {
        sleep 5
      }
    }
    stage('Upgrade') {
      steps {
        sleep 14
      }
    }
  }
}