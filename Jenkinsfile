pipeline {
  agent any
  stages {
    stage('version') {
      steps {
        sh '/etc/profile.d/rh-ruby27.sh'
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
        sh 'which -a ruby'
      }
    }
  }
}
