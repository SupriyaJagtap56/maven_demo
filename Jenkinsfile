pipeline {
  agent {
    docker {
      image 'maven:3.3.3'
      reuseNode true

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
        sh 'mvn install'
      }
    }

  }
}