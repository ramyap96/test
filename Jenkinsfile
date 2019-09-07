pipeline {
  agent any
  stages {
    stage('stage1') {
      parallel {
        stage('stage1') {
          steps {
            echo 'pipeline'
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
        echo 'end'
      }
    }
    stage('buildstage') {
      steps {
        build(job: 'test1', propagate: true)
      }
    }
  }
}