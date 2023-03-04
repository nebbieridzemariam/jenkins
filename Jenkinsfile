pipeline {
  agent any
  stages {
    stage('Checkout') {
      steps {
        sh 'git checkout -b blueOceanBranch1'
      }
    }

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