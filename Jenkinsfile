pipeline {
  agent any
  stages {
    stage('Upload Package') {
      steps {
        echo 'Upload Package'
        sleep 5
      }
    }
    stage('Register') {
      steps {
        echo 'Register'
        sleep 5
      }
    }    
    stage('Prepare') {
      parallel {       
        stage('Configuration') {
          steps {
            echo 'Configuration'
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
        echo 'A/B Test'
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
