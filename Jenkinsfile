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
      }
    }

    stage('go') {
      steps {
        tool(name: '1.19', type: 'go')
      }
    }

    stage('echo go version') {
      steps {
        sh 'go version'
      }
    }

  }
}