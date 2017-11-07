pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'bat \'mvn --version\''
      }
    }
    stage('Test') {
      steps {
        sh 'bat `mvn test`'
      }
    }
    stage('Deliver') {
      steps {
        sh 'bat \'./jenkins/scripts/deliver.sh\''
      }
    }
  }
}