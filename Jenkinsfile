pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'This is Building'
        sh 'docker rm -f `docker ps -a -q`'
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
  environment {
    PATH = "$PATH:/usr/local/bin"
  }
}