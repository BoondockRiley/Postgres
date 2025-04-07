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
            sh './runme.sh'
            sh 'liquibase flow'
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
