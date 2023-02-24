pipeline {
  agent {
    docker {
      image 'node:lts-alpine'
      args '-p 3000:3000'
    }

  }
  stages {
    stage('Build') {
      steps {
        sh 'npm install'
        git(url: 'https://github.com/radheysh/creating-a-pipeline-in-blue-ocean.git', branch: 'master')
      }
    }

  }
}