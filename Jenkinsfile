pipeline {
  agent any
  stages {
    stage('checks code') {
      steps {
        git(url: 'https://github.com/AkzholS7/jenkins.git', branch: 'main')
      }
    }

    stage('Log') {
      parallel {
        stage('Log') {
          steps {
            sh 'ls -la'
          }
        }

        stage('Front-End Unit Test') {
          steps {
            sh 'cd curriculum-front && npm i && npm run test:unit'
          }
        }

      }
    }

  }
}