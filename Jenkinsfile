pipeline {
  agent any
  environment {
        PATH = "$PATH:/usr/local/bin"
    }
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
      environment {
        PATH = '/usr/local/bin'
      }
      steps {
        sh 'docker-compose up -d'
      }
    }

  }
}