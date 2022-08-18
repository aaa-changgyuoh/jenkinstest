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

    stage('go') {
      steps {
        tool(name: '1.19', type: 'go')
      }
    }

  }
}