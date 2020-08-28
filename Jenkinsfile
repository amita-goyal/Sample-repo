pipeline {
  agent any
  stages {
    stage('GIT') {
      steps {
        build 'TX-automate_RunDevelopmentProjectBuild'
      }
    }

    stage('TX_TestCases') {
      parallel {
        stage('TX_Web') {
          steps {
            build 'TX-automate_WebTestCases'
          }
        }

        stage('TX_API') {
          steps {
            build 'TX-automate_APITestCases'
          }
        }

        stage('TX_Mobile') {
          steps {
            build 'TX-automate_MobileTestCases'
          }
        }

      }
    }

    stage('TX_Performance') {
      steps {
        build 'TX-automate_Performance'
      }
    }

    stage('TX_SonarQube') {
      steps {
        build 'TX-automate_SonarQube'
      }
    }

  }
}