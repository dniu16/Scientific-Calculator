pipeline {
  agent any
  stages {
    stage('Test') {
      steps {
        sh '''cd Calculator
mvn sonar:sonar \\
  -Dsonar.projectKey=calculator \\
  -Dsonar.host.url=http://localhost:9000 \\
  -Dsonar.login=c42a4e9f88871e563b112fb71945941a43d8897c
mvn test'''
      }
    }

  }
}