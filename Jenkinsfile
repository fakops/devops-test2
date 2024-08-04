pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'npm ci'
      }
    }

    stage('Unit Tests') {
      steps {
        sh 'npm run test:unit'
      }
    }

    stage('Integration Tests') {
      steps {
        sh 'npm run test:integration'
      }
    }

  }
}