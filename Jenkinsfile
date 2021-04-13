pipeline {
  agent any
  stages {
    stage('Test') {
      steps {
        sh '''cd Calculator
mvn clean install sonar:sonar'''
      }
    }

  }
}