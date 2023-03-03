pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh ' sh \'chmod +x build.sh && ./build.sh\''
        sh '''mvn clean test
'''
      }
    }

  }
}