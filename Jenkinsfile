pipeline {
  agent any
  stages {
    stage('git') {
      steps {
        git(url: 'https://github.com/sarath9985/files', changelog: true, branch: 'node', credentialsId: 's9491019985', poll: true)
      }
    }
    stage('deploy') {
      steps {
        sh '''npm install
npm start

'''
      }
    }
  }
}