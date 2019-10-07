pipeline {
  agent any
  stages {
    stage('Clean') {
      parallel {
        stage('Clean') {
          steps {
            sh 'mvn clan'
          }
        }
        stage('install') {
          steps {
            sh 'mvn install'
          }
        }
      }
    }
  }
}