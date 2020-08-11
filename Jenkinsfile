pipeline {
  agent any
  stages {
    stage('GIT') {
      steps {
        build 'GIT'
      }
    }

    stage('UIPath_Tests') {
      steps {
        build 'UIPath_excel_Integration'
      }
    }

    stage('Performance_Test') {
      steps {
        build 'Performance_Tests'
      }
    }

  }
}