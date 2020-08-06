pipeline {
  agent any
  stages {
    stage('GIT') {
      steps {
        build 'GIT'
      }
    }

    stage('Python_RestAPITests') {
      steps {
        build 'Python_ApiTestCases'
      }
    }

    stage('Python_WebTests') {
      steps {
        build 'Python_WebTestCases'
      }
    }

    stage('Python_MobileTests') {
      steps {
        build 'Python_MobileTestCases'
      }
    }

    stage('Generating_Reports') {
      steps {
        build 'Python_ReportGeneration'
      }
    }

  }
}