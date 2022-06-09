pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh '''pwd
ls
date'''
      }
    }

    stage('Test') {
      parallel {
        stage('Test') {
          steps {
            echo 'test step'
          }
        }

        stage('test par') {
          steps {
            echo 'test par'
          }
        }

      }
    }

    stage('Deploy') {
      steps {
        echo 'deploy done'
      }
    }

  }
}