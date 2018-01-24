pipeline {
  agent any
  stages {
    stage('Prepare') {
      parallel {       
        stage('Check Conflict') {
          steps {
            echo 'Check Conflict'
            sleep 10
          }
        }
        stage('Check Environment ') {
          steps {
            echo 'Check Environment'
            sleep 10
          }
        }
      }
    }
    stage('SandBox Test') {
      steps {
        echo 'Running SandBox Testing'
        sleep 5
      }
    }
    stage('Deploy') {
      steps {
        echo 'Deploy'
        sleep 5
      }
    }
    stage('A/B Test') {
      steps {
        echo 'Running A/B Test'
        sleep 5
      }
    }
    stage('Upgrade') {
      steps {
        echo 'Upgrade'
        sleep 15
      }
    }
  }
}
