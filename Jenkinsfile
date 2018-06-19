pipeline {
  agent any
  stages {
    stage('Print thing') {
      steps {
        echo 'Thing'
      }
    }
    stage('java') {
      steps {
        sh 'java -version'
      }
    }
  }
}