pipeline {
  agent any
  stages {
    stage('Build') {
      parallel {
        stage('Version') {
          steps {
            sleep 2
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