pipeline {
  agent any
  
  tools {
      nodejs 'node-11.0.0'
  }

  options {
    timeout(time: 2, unit: 'MINUTES')
  }

  stages {
    stage('install dependencies') {
      steps {
        script {
            sh 'npm i'
        }
      }
    }
    stage('run test') {
      steps {
        script {
            sh 'npm t'
        }
      }
    }
  }
}
