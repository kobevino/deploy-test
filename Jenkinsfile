pipeline {
  agent {
    docker {
      image 'node:10' 
      args '-p 3000:3000' 
    }
  }

  stages {
    stage('build') {
      steps {
        echo 'building the application'
        sh 'yarn'
        sh 'yarn build'
      }
    }

    stage('test') {
      steps {
        echo 'testing the application'
      }
    }

    stage('deploy') {
      steps {
        echo 'deploying the application'
      }
    }
  }
}
