pipeline {
  agent any
  environment {
        PATH = "$PATH:/usr/local/bin"
  }
  stages {
    stage('checkout project') {
      steps {
        checkout scm
      }
    }

    stage('start node docker') {
      steps {
        sh 'docker-compose up -d server'
      }
    }

  }
}