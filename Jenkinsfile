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
            bat '"C:\\Program Files\\Git\\bin\\bash.exe" -c "./runme.sh"'
            bat '"C:\\Program Files\\Git\\bin\\bash.exe" -c "liquibase flow"'
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