pipeline {
  agent any
  stages {
    stage('checkout code') {
      steps {
        git(url: 'https://github.com/chillugurisuryatejareddy/git_try_jenkins', branch: 'main')
      }
    }

    stage('log') {
      parallel {
        stage('end') {
          steps {
            sh 'ls -a'
          }
        }

        stage('front-end unit test') {
          steps {
            sh 'cd curriculum-front && npm i && npm run test:unit'
          }
        }

      }
    }

  }
}