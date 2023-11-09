pipeline {
  agent any
  stages {
    stage('Build') {
      parallel {
        stage('Version') {
          steps {
            sh '''java --version
mvn --version
git --version'''
          }
        }

        stage('error') {
          steps {
            echo 'Hello'
          }
        }

      }
    }

    stage('Deploy') {
      steps {
        echo 'Deploy'
      }
    }

    stage('Post') {
      steps {
        writeFile(file: 'C:\\Users\\sqwjng\\Desktop\\Jenkins\\Day4\\test.txt', text: 'It Work')
      }
    }

  }
}