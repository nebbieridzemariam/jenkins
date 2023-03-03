pipeline {
  agent any
  stages {
    stage('Functional Test') {
      steps {
        sh '''/opt/homebrew/Cellar/maven/3.9.0/libexec install
mvn clean test'''
      }
    }

  }
}