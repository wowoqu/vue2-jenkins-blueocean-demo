pipeline {
  agent {
    docker {
      image 'node'
      args '-p 3000:3000'
    }

  }
  stages {
    stage('Build') {
      steps {
        sh 'npm config set registry http://registry.npm.taobao.org'
        sh 'npm install'
      }
    }

  }
}