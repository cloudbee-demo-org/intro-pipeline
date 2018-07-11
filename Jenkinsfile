pipeline {
  agent {
    label 'jdk9'
  }
  stages {
    stage('Hello World') {
      steps {
        sh 'java -version'
        echo "Hello ${MY_NAME}"
        echo "${TEST_USER_USR}"
        echo "${TEST_USER_PSW}"
      }
    }
  }
  environment {
    MY_NAME = 'Mian'
    TEST_USER = credentials('test-user')
  }
  parameters {
    string(name: 'Name', defaultValue: 'whoever you are', description: 'Who should I say hi to?')
  }
}