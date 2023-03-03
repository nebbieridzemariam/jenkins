pipeline {
  agent any
  stages {
    stage('Functional Test') {
      steps {
        sh '''/opt/homebrew/bin/mvn install
mvn test clean'''
      }
    }

  }
}