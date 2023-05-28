pipeline {
  agent any
  stages {
    stage('Checkout Code') {
      steps {
        git(url: 'https://github.com/IkennaU/curriculum-app-dev.git', branch: 'main')
      }
    }

    stage('Logs') {
      steps {
        bat 'dir'
      }
    }

  }
}