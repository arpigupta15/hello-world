pipeline {
   agent any 
  stages ('CI') {
    stage('Checkout') {
      steps {
        echo 'Checkout'
        checkout scm
      }
    }
    stage('Build') {
      steps {
        // script
        sh 'mvn clean install'
      }
    }
    stage('Test') {
      steps {
        // script
        echo 'test'
        sh 'mvn test'
      }
    }
  }
}
