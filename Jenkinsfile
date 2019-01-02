pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'Clean insatll'
      }
    }
    stage('test') {
      parallel {
        stage('test') {
          steps {
            echo 'tests running'
          }
        }
        stage('test1') {
          steps {
            echo 'bdd'
          }
        }
      }
    }
    stage('Deploy') {
      steps {
        echo 'deploy code'
      }
    }
    stage('scan') {
      steps {
        echo 'scan code'
      }
    }
  }
}