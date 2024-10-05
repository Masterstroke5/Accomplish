pipeline {
  agent any
  stages {
    stage('Test') {
      parallel {
        stage('Test') {
          steps {
            echo 'Hello Test, This is the first stage of pipeline create by blue ocean'
            sh '''pwd
ls
date
'''
          }
        }

        stage('parallel job') {
          steps {
            echo 'This is parallel job create by blue ocean'
          }
        }

      }
    }

    stage('Github') {
      steps {
        sleep 30
      }
    }

  }
  environment {
    name = 'karishma'
  }
}