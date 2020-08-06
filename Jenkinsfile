pipeline {
  agent any
  stages {
    stage('GIT') {
      steps {
        build 'GIT'
      }
    }

    stage('Rest_API_Tests') {
      steps {
        build 'Python_ApiTestCases'
      }
    }

    stage('Web_Tests') {
      steps {
        build 'Python_WebTestCases'
      }
    }

    stage('Mobile_Tests') {
      steps {
        build 'Python_MobileTestCases'
      }
    }

    stage('Performance_Test') {
      steps {
        build 'Performance_Tests'
      }
    }

    stage('Generate Reports') {
      steps {
        build 'Python_ReportGeneration'
      }
    }

  }
}