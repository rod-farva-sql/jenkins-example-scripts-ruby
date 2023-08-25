pipeline {
  agent any
  stages {
    stage('version') {
      steps {
         sh 'ls -lah /opt/rh/rh-ruby27/root/bin/'
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
