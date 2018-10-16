pipeline {
  agent {
    node {
      label 'slave01'
    }

  }
  stages {
    stage('git') {
      steps {
        git(url: 'https://github.com/sarath9985/files', branch: 'node')
      }
    }
    stage('deploy') {
      steps {
        sh '''npm install
npm start'''
      }
    }
  }
}