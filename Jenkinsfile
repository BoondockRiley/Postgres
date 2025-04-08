pipeline {
  agent any
  stages {
    stage('Git') {
      parallel {
        stage('Git') {
          steps {
            echo 'Start'
          }
        }

        stage('Flow') {
          steps {
            echo 'LB - Flow'
            sh '''
              export PATH=/opt/homebrew/bin:$PATH
              liquibase flow
            '''
          }
        }

      }
    }

    stage('Test') {
      steps {
        echo 'End'
      }
    }

  }
}