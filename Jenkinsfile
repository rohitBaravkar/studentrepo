pipeline {
  agent any
  stages {
    stage('build') {
      agent any
      steps {
        sh 'mvn package'
      }
    }
    stage('test') {
      steps {
        sh 'mvn test'
      }
    }
  }
}