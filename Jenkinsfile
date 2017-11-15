pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        bat 'echo "Building"'
      }
    }
    stage('Test') {
      steps {
        sh 'bat `mvn test`'
      }
    }
    stage('Deliver') {
      steps {
        git 'https://github.com/Hirondina/1.git'
      }
    }
  }
}