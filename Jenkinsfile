pipeline {
  agent any
  stages {
    stage('Checkout Code') {
      steps {
        git(url: 'https://github.com/IkennaU/curriculum-app-dev.git', branch: 'main')
      }
    }

    stage('Logs') {
      parallel {
        stage('Logs') {
          steps {
            bat 'dir'
          }
        }

        stage('Front-End Unit Tests') {
          steps {
            bat 'cd curriculum-front && npm i && npm run test:unit'
          }
        }

      }
    }

  }
}