pipeline {
  agent any
  stages {
    stage('Build') {
      parallel {
        stage('Build') {
          steps {
            echo 'Hello'
          }
        }

        stage('Testing') {
          steps {
            echo 'Testing started'
          }
        }

      }
    }

    stage('Deploy') {
      steps {
        sleep 5
      }
    }

    stage('Post') {
      steps {
        writeFile(file: 'C:\\Users\\sqthwoon\\Desktop\\Jenkins\\BlueOcean.txt', text: 'completed')
      }
    }

  }
}