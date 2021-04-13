pipeline {
  agent any
  stages {
    stage('Test') {
      steps {
        sh '''cd Calculator
git pull
mvn clean install sonar:sonar -Dsonar.login=8afb4411f22bd1f43b08d28ad87b0faadc784dc2 -Dsonar.host.url=http://localhost:9000'''
      }
    }

  }
}