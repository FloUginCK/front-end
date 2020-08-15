pipeline {
  agent any
  tools {
    maven 'nodejs 4.8.6'
  }
  stages {
    stage('build') {
      steps {
        sh 'npm install'
      }
    }

    stage('test') {
      steps {
        sh 'npm test'
      }
    }

    stage('package') {
      steps {
        sh 'npt run package'
      }
    }

  }
}