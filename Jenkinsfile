pipeline {
  agent {
    label 'jdk8'
  }
  stages {
    stage('Print thing') {
      steps {
        echo "Hello  ${MY_NAME}"
      }
    }
    stage('java') {
      steps {
        sh 'java -version'
      }
    }
  }
  environment {
    MY_NAME = 'Jimmy'
  }
}