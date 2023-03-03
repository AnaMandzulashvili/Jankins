pipeline {
  agent any
  stages {
    stage('error') {
      parallel {
        stage('stage1') {
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