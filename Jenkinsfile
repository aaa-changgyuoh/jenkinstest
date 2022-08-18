pipeline {
  agent any
  stages {
    stage('Show Go version') {
      steps {
        sh 'go version'
      }
    }

    stage('Compile') {
      steps {
        sh 'go build'
      }
    }

    stage('build output') {
      steps {
        archiveArtifacts 'jenkinstest'
      }
    }

  }
  tools {
    go '1.19'
  }
  environment {
    GO111MODULE = 'on'
  }
}