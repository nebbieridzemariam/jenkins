pipeline {
  agent any
  stages {
    stage('Build') {
      parallel {
        stage('Build') {
          steps {
            sh 'mvn clean test'
          }
        }

        stage('Check Mvn Version') {
          steps {
            sh 'mvn -version'
          }
        }

      }
    }
stage('Checkout') {
            steps {
                checkout scm
                sh 'git checkout mariamo'
            }
        }
  }
  tools {
    maven 'Maven 3.9.0'
  }
}
