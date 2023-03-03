pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'mvn clean test'
      }
    }
    stage('Checkout') {
            steps {
                checkout scm
                sh 'git checkout New Branch'
            }
        }

  }
  tools {
    maven 'Maven 3.9.0'
  }
  
}
