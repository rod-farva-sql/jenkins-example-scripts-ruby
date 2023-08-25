pipeline {
  agent any
  stages {
    stage('version') {
      steps {
         sh '/etc/profile.d/rh-ruby27.sh'
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
