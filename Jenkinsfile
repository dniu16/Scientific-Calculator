pipeline {
  agent any
  stages {
    stage('Test') {
      steps {
        sh '''cd Calculator
git pull
mvn clean install sonar:sonar'''
      }
    }

  }
}