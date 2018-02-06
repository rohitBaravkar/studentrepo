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
    stage('run java app') {
      steps {
        sh '''cd /var/lib/jenkins/workspace/studentrepo_master-LDD7RJLB5AFD7XXZX5IH4KSYC7MNI6ZU3O4NLIGNXHFJ6PQ5LRPA@2/target/
ls
java -jar StudentMgmnt-0.0.1-SNAPSHOT.jar'''
      }
    }
  }
}
