pipeline {
  agent any
  stages {
    stage('stages') {
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