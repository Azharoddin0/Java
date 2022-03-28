pipeline {
  agent any
  stages {
    stage('Test') {
      steps {
        sh '''cal 2022
echo\'hi\''''
      }
    }

    stage('Build') {
      parallel {
        stage('Build') {
          steps {
            echo 'can we proceed'
          }
        }

        stage('sub-Build') {
          steps {
            sh 'pwd'
          }
        }

      }
    }

    stage('Deploy for test') {
      steps {
        sh 'cal 2023'
      }
    }

  }
}