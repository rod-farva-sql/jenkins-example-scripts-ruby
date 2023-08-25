pipeline {
  agent any
  stages {
    stage('version') {
      steps {
         source '/etc/profile'
         sh 'echo $PATH'
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
