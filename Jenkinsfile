pipeline {
  agent any
  stages {
    stage('version') {
      steps {
        sh 'ruby --version'
      }
    }
    stage('hello') {
      steps {
        sh 'ruby Hello.rb'
      }
    }
    stage('which') {
      steps {
        sh 'which ruby'
      }
    }
  }
}
