pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'mvn clean test'
      }
    }

  }
  tools {
    maven 'Maven 3.9.0'
  }
}