node {
    // Define the desired Ruby path
    def rubyPath = "/opt/rh/rh-ruby27/root/usr/bin"

    // Inject environment variables
    wrap([$class: 'EnvInjectBuildWrapper', 
          // Adding the Ruby path to the existing PATH
          buildEnvVars: [PATH+':'+rubyPath]]) {
              

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

    }
}
