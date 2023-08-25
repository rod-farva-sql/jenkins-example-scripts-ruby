pipeline {
  agent any
      
  stages {
    stage('version') {
      steps {
         sh 'ruby -v'
      }
    }
    stage('hello') {
      steps {
        sh 'ruby Hello.rb'
      }
    }
    stage('which') {
      steps {
        sh 'which -a ruby'
      }
    }
  }
}


