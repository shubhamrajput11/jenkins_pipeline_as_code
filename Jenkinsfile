pipeline {
  agent any
  stages {
    stage('helloworld') {
      steps {
        sh 'echo "Hello world"'
      }
    }

    stage('user') {
      parallel {
        stage('user') {
          steps {
            sh 'whoami'
          }
        }

        stage('pwd') {
          steps {
            sh 'pwd'
          }
        }

      }
    }

  }
}