pipeline {
  agent any

  stages {
    stage ('Verify') {
      agent {
        docker {
          alwaysPull true
          reuseNode true
          image 'maven:3.8.7-openjdk-18'
        }
      }
      steps {
          sh 'mvn -version'
      }
    }
  }
}
   

