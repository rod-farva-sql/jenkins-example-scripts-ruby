pipeline {
  agent any

  environment {
    PATH = "/opt/rh/rh-ruby27/root/usr/local/bin:/opt/rh/rh-ruby27/root/usr/bin:/usr/local/bin:/usr/bin:/usr/local/sbin:/usr/sbin:/home/centos/.local/bin:/home/centos/bin"
  }
      
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

