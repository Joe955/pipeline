pipeline {
  agent any
  stages {
    stage('Upload Package') {
      agent {
        node {
          label 'Upload Package'
        }
        
      }
      steps {
        sh 'ls'
      }
    }
    stage('Register') {
      agent {
        node {
          label 'Register'
        }
        
      }
      steps {
        sh 'ls'
      }
    }
    stage('Configuration') {
      agent {
        node {
          label 'Configuration'
        }
        
      }
      steps {
        echo 'Config'
      }
    }
    stage('SandBox Test') {
      steps {
        waitUntil() {
          sleep 1
          sh 'ls'
        }
        
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