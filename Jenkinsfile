pipeline {
  agent any
  stages {
    stage("build") {
      steps {
        sh """
          docker build -t alpine-linux .
        """
      }
    }
    stage("run") {
      steps {
        sh """
          docker run --rm alpine-linux 
        """
      }
    }
  }
}
