pipeline {
  agent {
    label 'jdk8'
  }
  stages {
    stage('Print thing') {
      steps {
        echo "Hello  ${params.Name}"
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
  parameters {
    string(name: 'Name', defaultValue: 'whoever you are', description: 'Who should I say hi to?')
  }
}