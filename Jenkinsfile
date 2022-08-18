pipeline {
  agent any
   tools { go '1.19' }
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
      }
    }

    stage('echo go version') {
      steps {
        sh 'go version'
      }
    }

  }
}