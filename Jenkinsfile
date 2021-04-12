pipeline {
  agent any
  stages {
    stage('Test') {
      steps {
        sh '''cd Calculator
mvn sonar:sonar -Dsonar.projectKey=calculator -Dsonar.host.url=http://localhost:9000
mvn test'''
      }
    }

  }
}