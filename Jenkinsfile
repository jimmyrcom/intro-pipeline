pipeline {
  agent {
    label 'jdk8'
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