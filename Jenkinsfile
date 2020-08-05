pipeline {
  agent any
  stages {
    stage('GIT') {
      steps {
        build 'GIT'
      }
    }

    stage('Python_Tests') {
      steps {
        build 'Python_TestCases'
      }
    }

  }
}