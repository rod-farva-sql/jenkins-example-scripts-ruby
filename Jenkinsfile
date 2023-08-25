pipeline {
  agent any
  stages {
    stage('version') {
      steps {
         sh '/opt/rh/rh-ruby27/root/usr/bin/ruby --version'
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
