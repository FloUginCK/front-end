pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        sh 'npm install'
        nodejs 'nodejs 4.8.6'
      }
    }

    stage('test') {
      steps {
        sh 'npm test'
      }
    }

    stage('package') {
      steps {
        sh 'npm run package'
      }
    }

  }
}