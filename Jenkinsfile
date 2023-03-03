pipeline {
  agent any
  stages {
    stage('error') {
      parallel {
        stage('error') {
          steps {
            bat(script: 'mvn clean test', returnStatus: true)
          }
        }

        stage('stage 2') {
          steps {
            bat(script: 'mvn version', returnStatus: true)
          }
        }

      }
    }

  }
}