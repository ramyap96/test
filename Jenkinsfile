pipeline {
  agent any
  stages {
    stage('stage1') {
      parallel {
        stage('stage1') {
          steps {
            sh '''echo"hai"

'''
          }
        }
        stage('stage2') {
          steps {
            echo 'pipeline'
          }
        }
      }
    }
    stage('bluestage') {
      steps {
        sh 'end'
      }
    }
  }
}