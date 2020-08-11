pipeline {
  agent any
  stages {
    stage('GIT') {
      steps {
        build 'RunDevelopmentProject'
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