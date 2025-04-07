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
            sh 'echo $PATH'
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