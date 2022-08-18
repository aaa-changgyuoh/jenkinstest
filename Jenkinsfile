pipeline {
  agent any
  stages {
    stage('Show Go version') {
      steps {
        sh 'go version'
      }
    }

    stage('Build a project') {
      steps {
        build 'build a project'
      }
    }

  }
  tools {
    go '1.19'
  }
}