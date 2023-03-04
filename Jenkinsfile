pipeline {
  agent any
  stages {
    stage('Checkout') {
      steps {
        sh 'git checkout -b blueOceanBranch2'
      }
    }

    stage('Build') {
      parallel {
        stage('Build') {
          steps {
            sh 'mvn clean test'
          }
        }

        stage('Check MVN') {
          steps {
            sh 'mvn -version'
          }
        }

      }
    }

  }
  tools {
    maven 'Maven 3.9.0'
  }
}