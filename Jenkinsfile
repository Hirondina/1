pipeline {
  agent any
  stages {
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