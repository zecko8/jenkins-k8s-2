pipeline {
  agent any
  stages {
    stage('check file') {
      steps {
        sh 'pwd'
        sh 'ls -l'
      }
    }
    stage('run') {
      steps {
        sh '/bin/bash prova.sh'
      }
    }
  }
}
