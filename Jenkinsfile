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
            bat '"C:\\Program Files\\Git\\bin\\bash.exe" -c "liquibase --version"'
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