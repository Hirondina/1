pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh '\'mvn -B -DskipTests clean package\''
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