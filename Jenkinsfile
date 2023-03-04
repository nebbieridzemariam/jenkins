pipeline {
  agent any
  stages {
    stage('Checkout') {
      steps {
        sh 'git checkout -b blueOceanBranch1'
      }
    }

  }
  tools {
    maven 'Maven 3.9.0'
  }
}