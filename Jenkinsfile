pipeline {
  agent any
  stages {
    stage('Functional Test') {
      parallel {
        stage('Functional Test') {
          steps {
            bat 'mvn clean test'
          }
        }

        stage('Maven Version') {
          steps {
            bat 'mvn --version'
          }
        }

      }
    }

  }
}