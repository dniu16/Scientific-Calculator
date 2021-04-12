pipeline {
  agent any
  stages {
    stage('Test') {
      steps {
        sh '''cd Calculator
mvn sonar:sonar \\
  -Dsonar.projectKey=calculator \\
  -Dsonar.host.url=http://192.168.1.37:9000 \\
  -Dsonar.login=6c5fe8d2c9ce97018a385951bb45a0e8c4b6c8bf
mvn test'''
      }
    }

  }
}