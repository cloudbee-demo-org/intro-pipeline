pipeline {
  agent {
    label 'jdk9'
  }
  stages {
    stage('Hello World') {
      steps {
        sh 'java -version'
        echo "Hello ${MY_NAME}"
      }
    }
  }
  environment {
    MY_NAME = 'Mian'
  }
}