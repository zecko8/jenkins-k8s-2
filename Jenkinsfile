pipeline {
  agent any
  stages {
    stage('check file') {
      steps {
        sh 'pwd'
        sh 'ls -l'
      }
    }
    stage('build') {
      steps {
        sh 'docker build -t image-prova-sh . '
        sh 'docker images'
      }
    }
    stage('run') {
      steps {
        sh 'docker run image-prova-sh /bin/bash prova.sh && ls '
      }
    }
  }
}
