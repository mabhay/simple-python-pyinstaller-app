pipeline {
  agent any
  stages {
    stage('Git Pull') {
      steps {
        git(url: 'https://github.com/mabhay/simple-python-pyinstaller-app.git', branch: 'master', credentialsId: 'mabhay')
      }
    }

    stage('Unit Test') {
      steps {
        sh 'echo \'Hello in Unit Test\''
      }
    }

    stage('Integration Test') {
      steps {
        sh 'echo \'Hello in Integration Test\''
      }
    }

  }
  environment {
    Testing = 'Unit'
  }
}