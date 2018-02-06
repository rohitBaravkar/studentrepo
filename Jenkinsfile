pipeline {
  agent any
  stages {
    stage('build') {
      agent any
      steps {
        sh 'mvn deploy'
      }
    }
    stage('test') {
      steps {
        sh 'mvn test'
      }
    }
  }
}