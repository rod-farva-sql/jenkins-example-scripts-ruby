pipeline {
  agent any
  stages {
    stage('version') {
      steps {
         sh 'source /opt/rh/rh-ruby27/enable'
         sh '/opt/rh/rh-ruby27/root/usr/bin/ruby -v'
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
