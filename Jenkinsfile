pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        sh '''pwd
date
'''
      }
    }

    stage('test') {
      steps {
        echo 'testing'
        sh 'ls'
      }
    }

    stage('deploy') {
      parallel {
        stage('deploy') {
          steps {
            echo 'deploying'
          }
        }

        stage('deploy parallel') {
          steps {
            sh 'ls'
          }
        }

      }
    }

  }
}