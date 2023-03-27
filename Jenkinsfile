pipeline {
  agent any
  stages {
    stage('checks code') {
      steps {
        git(url: 'https://github.com/AkzholS7/jenkins.git', branch: 'main')
      }
    }

    stage('Log') {
      steps {
        sh 'ls -la'
      }
    }

  }
}