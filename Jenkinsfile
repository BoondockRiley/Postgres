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

        stage('') {
          steps {
            echo 'LB - Flow'
            
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