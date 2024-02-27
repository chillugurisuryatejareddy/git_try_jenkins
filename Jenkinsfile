pipeline {
  agent any
  stages {
    stage('checkout code') {
      steps {
        git(url: 'https://github.com/chillugurisuryatejareddy/git_try_jenkins', branch: 'main')
      }
    }

    stage('end') {
      steps {
        sh 'ls -a'
        echo 'task ended'
      }
    }

  }
}