pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'This is Building'
      }
    }

    stage('Test') {
      steps {
        echo 'This is Testing'
      }
    }

    stage('Deploy') {
      steps {
        sh 'docker-compose up -d'
      }
    }

  }
}