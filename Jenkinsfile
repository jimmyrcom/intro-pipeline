pipeline {
  agent {
    label 'jdk9'
  }
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