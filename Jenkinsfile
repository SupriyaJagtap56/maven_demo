pipeline {
  agent {
    docker {
      image 'maven:3.3.3'
    }

  }
  stages {
    stage('Log') {
      steps {
        echo 'Log version info'
        sh 'mvn --version'
      }
    }

    stage('Build') {
      steps {
        sh 'mvn build'
      }
    }

  }
}