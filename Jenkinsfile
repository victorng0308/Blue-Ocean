pipeline {
  agent any
  stages {
    stage('Version') {
      steps {
        sh '''java --version
mvn --version
git --version'''
      }
    }

    stage('File') {
      steps {
        bat(script: 'test.txt', label: 'completed')
      }
    }

  }
}