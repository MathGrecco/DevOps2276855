pipeline {
  agent any
  stages {
    stage("verify tooling") {
      steps {
          sh '''

          docker info
          docker version
          docker compose version
          java --version
          docker-compose build
          docker-compose up

          '''
      }
    }
  }
}