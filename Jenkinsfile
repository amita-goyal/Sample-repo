pipeline {
  agent any
  stages {
    stage('GIT') {
      steps {
        build 'RunDevelopmentProject'
      }
    }

    stage('Python Tests') {
      steps {
        build 'Python_WebTests'
      }
    }

    stage('Performance Scripts') {
      steps {
        build 'UiPathPerformance'
      }
    }

  }
}