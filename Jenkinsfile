pipeline {
  agent any
      
  stages {
    stage('version') {
      steps {
         sh '/opt/rh/rh-ruby27/root/usr/bin/ruby -v'
      }
    }
    stage('hello') {
      steps {
        sh '/opt/rh/rh-ruby27/root/usr/bin/ruby Hello.rb'
      }
    }
    stage('which') {
      steps {
        sh 'which -a ruby'
      }
    }
  }
}


