pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'building the software'
        sh 'npm install'
      }
    }

    stage('Unit Tests') {
      steps {
        echo 'Running unit tests'
        sh 'npm run test:unit'
      }
    }

    stage('Integration Tests') {
      steps {
        echo 'Running integration tests'
        sh 'npm run test:integration'
      }
    }

  }
}