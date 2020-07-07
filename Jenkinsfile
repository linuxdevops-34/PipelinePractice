pipeline {
  agent any
  stages {
    stage('build') {
      parallel {
        stage('build') {
          steps {
            sh 'echo \'i am building a code here\''
          }
        }

        stage('Test') {
          steps {
            echo 'testing here'
          }
        }

      }
    }

    stage('deploy') {
      steps {
        echo 'I am deploying code here'
      }
    }

  }
}