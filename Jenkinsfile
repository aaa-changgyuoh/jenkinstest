pipeline {
  agent any
  stages {
    stage('LocalBuild') {
      steps {
        echo 'Starting Local Build...'
      }
    }

    stage('Echo Path') {
      steps {
        sh '''echo $PATH
echo $HOME'''
        sh 'go version'
      }
    }

  }
}