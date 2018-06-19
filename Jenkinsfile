pipeline {
  agent {
    label 'jdk8'
  }
  stages {
    stage('Print thing') {
      steps {
        echo "Hello  ${MY_NAME}"
        echo "${TEST_USER_USR}"
        echo "${TEST_USER_PSW}"
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
    TEST_USER = credentials('test-user')
  }
}